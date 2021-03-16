# flask-ml-app
AppEngine ML Application

[1]

export PROJECT_ID=[YOUR_PROJECT_ID]

[2]

create a service account with permission

download the json key and attach in the file

[3]

virtualenv -p python3 env

source env/bin/activate

pip install -r requirements.txt

[4]

gcloud app create

export GOOGLE_APPLICATION_CREDENTIALS="key.json"

[5]

export CLOUD_STORAGE_BUCKET=<bucket name for storage>

---
for local test

python main.py
----
[6]
app.yaml add gcs bucket name

[7]

gcloud app deploy



----
Load testing of App Engine
----
search "lamp stack" in search menu
launch machine; do ssh 

ab -V

ab -n 2 -c 1 https://housing-project-304202.ue.r.appspot.com/

ab -n 1000 -c 4 http://housing-project-304202.ue.r.appspot.com/

ab -n 16000 -c https://housing-project-304202.ue.r.appspot.com/
