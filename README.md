# dghorai-portfolio-projects
This is my personal website consisting of portfolio projects.

URL: https://dghorai-flaskapp.herokuapp.com/


**Steps Followed to Deploy Python Flask App on Heroku:**
* Step-1: [Login Heroku](https://www.heroku.com/)
* Step-2: Select 'Create new app'
* Step-3: Download [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli) and installed
* Step-4: Go to project folder
  * Create following two files in the project folder
    * requirements.txt (list of the modules and packages required for the project)
    * Procfile (with File extention)
  * Open Procfile and then write the following line:
    * web: gunicorn app:app (here the first app is the python file app.py and the second app is the flask app a variable in app.py)
  * Select full path of the project folder and then type 'CMD' or open 'CMD' from the Windows Start Menu
  * Type 'git init' and press enter (this command creates an empty Git repository in the project folder)
  * Type 'heroku login' and press enter (this will open heroku login page)
  * Type 'heroku git:remote -a flask-app-name' and press enter (flask-app-name will be the name used in Create new app in the step-2)
  * Type 'pip install gunicorn' (this will install gunicorn package in the python virtual environment availale in project folder/some other directory)
  * Type 'pip freeze > requirements.txt' to get all the modules and packages actual version used for the project
  * Type 'git add .'
  * Type 'git commit -m "first commit"'
  * Type 'git push heroku master'
  * Type 'heroku open' (it will open web application)
* Done!
