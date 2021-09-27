python 3.8.6

sudo apt install python3-virtualenv

virtualenv -p python3 venv

source venv/bin/activate

pip install Flask-API

pip install flask-mongoengine https://pythonbasics.org/flask-mongodb/ https://flask-pymongo.readthedocs.io/en/latest/

pip install pyjwt

python app.py

The server will run on port 5000

About mongoDB: https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/ https://blog.e-zest.com/basic-commands-for-mongodb

About Docker: https://www.linuxtechi.com/install-use-docker-on-ubuntu/ https://stackoverflow.com/questions/48957195/how-to-fix-docker-got-permission-denied-issue

Save all python packages into requirements: pip freeze > requirements.txt

docker build -t backend .

docker run --rm -d --network host --name backend backend

docker run --rm -d --network host -v mongovol:/mongovolData --name mongo mongo

check mongo: service mongod status

https://www.guguweb.com/2019/02/07/how-to-move-docker-data-directory-to-another-location-on-ubuntu/

docker exec -it mongo bash
