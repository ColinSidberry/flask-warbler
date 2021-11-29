# Warbler
Flask made "Twitter-esk" clone. 

## Features Complete
- Login/Signup
- User can: 
    - view profiles, 
    - follow other users
    - create public messages
    - like messages

## Getting Up & Running
1. Flask Environment Setup
    ```console
    $ python3 -m venv venv
    $ source venv/bin/activate
    (venv) $ pip install -r requirements.txt
    ```
2. Database Setup
    ```console
    (venv) $ psql
    =# CREATE DATABASE warbler;
    =# (control-d)
    (venv) $ python seed.py
    ```
3. .env File Setup

    Add the following lines to your .env file:
    ```txt
    SECRET_KEY=fake_key
    DATABASE_URL=postgresql:///warbler
    ```
4. Run the Server
    ```console
    (venv) $ flask run
    ```

## Database Models
![db_models_diagram](./db_models_diagram.jpg)

## Features Outstanding
- Sending direct messages
- Allow admin users

## Dev Roadmap
1. Ensure comprehensive testing (priority: add testing for message model)
2. Make mobile friendly
    - Fix alignment of profile image in a message.
    - Message spacing on mobile
    - Logout button placement on mobile
6. Fix profile picture
7. Optimize SQL Query counts
