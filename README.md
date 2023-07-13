# Django project template

## Project setup (Local Environment)

- Clone the repository: https://github.com/CodeForTravel/django_template.git
  ```sh
  git clone https://github.com/CodeForTravel/django_template.git
  ```
- Create a .env file inside the project directory and copy from .envs/.local/.django to .env and set the environment variables according to the needs.

- Create a virtual environment named like env with Python's venv

  ```sh
  python3 -m venv env
  ```

  - Activate the virtual environment (For Ubuntu):
    ```bash
    source env/bin/activate
    ```
  - For Windows:
    ```bash
    env\Scripts\activate
    ```

  ```

  ```

- Install all required packages:

  ```bash
  pip install -r requirements/local.txt
  ```

- Run below command to make .env file readable

  ```bash
  export DJANGO_READ_DOT_ENV_FILE=True
  ```

  - Run **migrate** command to propagate the migrations files into the db

  ```bash
  python manage.py migrate
  ```

  - Run Django server

  ```bash
  python manage.py runserver
  ```

- Create admin account if needed

  ```
  python manage.py createsuperuser
  ```

  ## Makefile

- Delete `.pyc` files with the command:

  ```bash
  make clean
  ```
