# flask_food_review
A python flask sqlAlchemy restaurant review site project

This is based on Miguel Grinberg's Udemy course - Flask Mega-Tutorial
Also check out https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world
Other info gleaned from:
Rafeh Qazi, aka, Clever Programmer YouTube, Python Flask Tutorial for Beginners
Anthony Herbert, Pretty Printed YouTube, Flask SQLAlchemy series of videos

# first steps for the python project
make a new project folder
command prompt cd c:\users\...\project_folder
python -m venv venv  # set up the virtual env
venv\Scripts\activate  # acitivate the virtual env
python -m pip install --upgrade pip # uninstalls pip-20.1.1 then install pip-20.2.2
pip install flask  # adds flask plus the packages it needs
python  # run python 
import flask  # check to see if flask is working, nothing happens unless there are errors
quit()	# close python interpretor and back to venv prompt

pip install Flask-SQLAlchemy  # Flask-SQLAlchemy==2.4.4
pip install Flask-Migrate  # Flask-Migrate==2.5.3

# factor out the different components of the application into a group of interconnected modules
flask_food_review/
  run.py  # the file invoked by flask run, be sure to 'Set FLASK_APP=run.py' (Set is for windows)
  app/  
    __init__.py
    config.py
    routes.py
    models.py
    forms.py
    static/
    templates/
      index.html
      
dunder init - initializes, executes and defines the app package and brings together all of the various components

config.py - configs baby

routes.py - where the routes are defined, routes are the different URLs that the application implements

models.py - where the models are defined, i.e., tables, fields and relationships

forms.py - where the forms are defined. The Flask-WTF extension uses Python classes to represent web forms. A form class simply defines the 
fields of the form as class variables
   
static/ - styling sheets and javascript

templates/ - where the Jinja2 templates which are html files with jinja2 notations, i.e., {% block head %} {% endblock %} (percent braces and double braces)

