# Chat Website to learn about Django, WebSockets, and Django Channels

This project demonstrates how to create a real-time chat website using Django and Django Channels. Follow this guide to set up the project, create users, and start chatting.

## Getting Started

### Prerequisites

Ensure you have Python and pip installed on your machine.

### Installation

1. **Create a virtual environment:**

    ```
    python3 -m venv venv
    ```

2. **Activate the virtual environment:**

    - On Windows:

        ```
        venv\Scripts\activate
        ```

    - On macOS and Linux:

        ```
        source venv/bin/activate
        ```

3. **Install dependencies:**

    ```
    pip install -r requirements.txt
    ```

### Change Directory

Ensure you are in the correct directory where the `manage.py` file is located:

```
cd core
```

### Database Migrations

Run the following command to apply the necessary database migrations:

```
python3 manage.py makemigrations
python3 manage.py migrate
```
### Create Superuser
Create a superuser to access the Django admin site:

```
python3 manage.py createsuperuser 
```
Follow the prompts to set the username, email, and password.

### Run the Development Server

Start the Django development server:
```
python3 manage.py runserver
```

### Access the Admin Site
Log in to the Django admin site to create additional users:
```
http://127.0.0.1:8000/admin/
```

### Access the Chat Application
Visit the main route, enter your username and the desired chat room:
```
http://127.0.0.1:8000/
```

WebSocket Connection
While sending messages, open the browser's developer tools (DevTools) console to monitor WebSocket connections and disconnections.

License
This project is licensed under the MIT License. See the [**LICENSE**](./LICENSE) file for details.