# pizzas

API for creating pizza orders and much more.

## Steps to run a local server

1. Install the required modules
   ```shell
    pip install -r requirements.txt
    ```
2. Make migrations
    ```shell
    python manage.py makemigrations pizza
    ```
3. Apply migrations
    ```shell
    python manage.py migrate
    ```
4. Run server
    ```shell
    python manage.py runserver
    ```
5. Go to http://127.0.0.1:8000/docs for testing the APIs.


## API Info

1. **create**
    <details><summary><ins>pizza</ins></summary>
    
    - POST `/api/create/pizza/`
    
        | Parameter  | Description |
        | ------------- | ------------- |
        | `pizza_type` **(required)** | Type of pizza (*i.e.* regular or square)  |
        | `pizza_size` **(required)** | Size of pizza (*e.g.* small, medium, large, etc.)  |
        | `topping` **(required)**    | Topping on the pizza (*e.g.* tomato, onion, cheese, corn, etc.)|
    
    
    </details>

    <details><summary><ins>topping </ins></summary>
    
    - POST `/api/create/topping/`
    
        | Parameter  | Description |
        | ------------- | ------------- |
        | `topping` **(required)**    | Topping on the pizza (*e.g.* tomato, onion, cheese, corn, etc.)|
        
    
    </details>

2. **list**
    <details>
    <summary><ins>all > list</ins></summary>
   
    - GET `/api/list/all/`
   
    </details>
    
    </details>

    <details>
    <summary><ins>all > size > list</ins></summary>
    
    - GET `/api/list/all/size/`
    
   
    </details>

    <details>
    <summary><ins>all > topping > list</ins></summary>
    
    - GET `/api/list/all/topping/`
    
    
    </details>

    <details><summary><ins>id > read</ins></summary>
    
    - GET `/api/list/{id}/`
    
        | Parameter  | Description |
        | ------------- | ------------- |
        | `id` **(required)** | Pizza ID  |
    
   
    </details>

    <details><summary><ins>size > read</ins></summary>
    
    - GET `/api/list/size/{size}/`
    
        | Parameter  | Description |
        | ------------- | ------------- |
        | `size` **(required)**    | Size of pizza |
    
  
  
    </details>

    <details><summary><ins>type > read</ins></summary>
    
    - GET `/api/list/type/{type}/`
    
        | Parameter  | Description |
        | ------------- | ------------- |
        | `type` **(required)**    | Size of pizza |
    
    
    </details>

3. **modify**
    <details>
    <summary><ins>read</ins></summary>
   
    - GET `/api/modify/{id}/`
   
    </details>
   
    <details>
    <summary><ins>update</ins></summary>
   
    - GET `/api/modify/{id}/`
    
    </details>