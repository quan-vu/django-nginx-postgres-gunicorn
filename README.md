# Deploy Django, Gunicorn, NGINX, Postgresql using Docker

# Project structure
  <project_root>
  		|__ config
  		|	|__ nginx
  		|   ...
  		|	
  		|__ src
  			...
  			<django_project_source>
  			...

# Tutorial

## Step 1 - Create a simple Django project inside "src" directory:
	```shell
	$ cd src
	$ virtualenv --python=python3 venv
	$ source venv/bin/activate
	(venv)$ pip install -r requirements.txt
	(venv)$ django-admin startproject mydjango
	(venv)$ python manage.py runserver
	```

	- Be sure your django project works at: http://127.0.0.1:8000/
	- If you get an error: "DisallowedHost", you may need to add '127.0.0.1' to ALLOWED_HOSTS.
	- Done.