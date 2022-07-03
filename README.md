# Senior Panel

Senior Panel is a web app that displays useful info for elderly people. The stack is composed of a Python Django Backend and a Bootstrap + Javascript frontend.

### Development requirements

You need to have Python installed to run the Django Server. The development version was 3.10.5. It is advisable to use [virtualenv](https://virtualenv.pypa.io/en/latest/) to isolate Python environments.

Once you have installed Python, download the package dependencies by executing:
```
pip install -r requirements
```
This will install Django and other package dependencies to run the server.

### How to run server?

Go to the root directory of the project and execute: 
```
python manage.py runserver 8080
```

This will start the server in the IP address: http://127.0.0.1:8080.

### Frontend

To update carousel sliding speed and image title delay, you need to change the following variables on the top of file **"senior_panel/static/senior_panel.js"**:

```
const kCarouselSlideInterval = 6000
const kCarouselTitleInterval = 3000
```

To update font-size, colors and other CSS attributes, change the file  **"senior_panel/static/senior_panel.css"**.

### Database

This project uses a simple **SQLite** database. The database is the file db.sqlite3 in the root. The commands to update migrations are described in the [Django docs](https://docs.djangoproject.com/en/4.0/topics/migrations/). 
