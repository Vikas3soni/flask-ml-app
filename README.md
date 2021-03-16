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
