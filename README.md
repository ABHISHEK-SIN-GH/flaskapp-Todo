# flaskapp-Todo

#cmd for run app in localserver(on windows)

<!--install virtual env-->

pip install virtualenv


<!--activate virtual env-->

.\env\sccripts\activate.ps1


<!--install modules-->

pip install flask
pip install sqlalchemy

set FLASK_APP=app.py


<!--for development mode-->

set FLASK_APP=ENV
flask run



#cmd for deploying website on heroku

heroku login

pip install gunicorn
pip freeze requirements.txt
Procfile
web:gunicorn app:app

git init
git add .
git commit -m "Initial commmit"

heroku create todo-codewithharry
git remote -v
git push heroku master
