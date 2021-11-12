# Warbler

Warbler is a flask made "Twitter-esk" clone. 

### Getting Up & Running
1. Python Envornment Setup
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
    SECRET_KEY=abc123
    DATABASE_URL=postgresql:///warbler
    ```
4. Run the Server
    ```console
    (venv) $ flask run
    ```
