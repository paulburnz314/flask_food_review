# flask_food_review
A python flask sqlAlchemy restaurant review site project

## Background
'''bash
This is based on Miguel Grinberg's Udemy course - Flask Mega-Tutorial
Also check out https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world
'''
'''bash
Other info gleaned from:
Rafeh Qazi, aka, Clever Programmer YouTube, Python Flask Tutorial for Beginners

Anthony Herbert, Pretty Printed YouTube, Flask SQLAlchemy series of videos
'''

## First steps for the python project
'''bash
make a new project folder
command prompt cd c:\users\...\project_folder
python -m venv venv  # set up the virtual env
venv\Scripts\activate  # acitivate the virtual env
python -m pip install --upgrade pip # uninstalls pip-20.1.1 then install pip-20.2.2
pip install flask  # adds flask plus the packages it needs
pip install Flask-SQLAlchemy  # Flask-SQLAlchemy==2.4.4
pip install Flask-Migrate  # Flask-Migrate==2.5.3
'''

# factor out the different components into a group of interconnected modules
'''bash
flask_food_review/run.py - the file invoked by flask run, be sure to 'Set FLASK_APP=run.py' (Set is for windows)
'''
'''bash
flask_food_review/app/__init__.py - dunder init executes and defines the app package and brings together all of the various components
'''   
dunder init - initializes, executes and defines the app package and brings together all of the various components

config.py - configs baby

routes.py - where the routes are defined, routes are the different URLs that the application implements

models.py - where the models are defined, i.e., tables, fields and relationships

forms.py - where the forms are defined. The Flask-WTF extension uses Python classes to represent web forms. A form class simply defines the 
fields of the form as class variables
   
static/ - styling sheets and javascript

templates/ - where the Jinja2 templates which are html files with jinja2 notations, i.e., {% block head %} {% endblock %} (percent braces and double braces)

