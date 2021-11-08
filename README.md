# flask-basic-app

- Set app main
export FLASK_APP=main.py

- to debbug:
export FLASK_DEBUG=1

- GCP commands:
### login gcloud 
gcloud init -> init the project
gcloud auth login -> login to gcp
gcloud auth application-default login -> login localy to interact with cloud from local enviroment

To revert your SDK to the previously installed version, you may run:
  $ gcloud components update --version 361.0.0

### Deploy to App Engine
1. create file: app.yaml ---> runtime: python37
2. create a project in gcp
3. select the project: gcloud init
4. execute: gcloud app deploy app.yaml ---> this will deploy de code
5. Make sure Firestore is activated in the same project space 
6. Execute: gcloud app browse ---> this will try to open the website in the browser
