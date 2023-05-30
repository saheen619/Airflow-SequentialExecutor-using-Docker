## Sequential Executor in Apache AirFlow using a Docker Container

### Apache Airflow

Apache Airflow is an open-source workflow management platform for data engineering and machine learning pipelines. It is used to programmatically schedule, and monitor workflows. Airflow uses DAG to represent workflows in a very interactive UI.

Workflow DAG:

![WORKFLOW_DAG](https://github.com/saheen619/Airflow-SequentialExecutor-using-Docker/blob/main/Documentation/Snips/DAG%20Running.JPG?raw=true)

### Sequential Executor in Apache Airflow   

The Sequential Executor is the default executor in Airflow. It is a local executor, where tasks are run on the same machine as the scheduler. Not very scalable kind of executor and not used for production. The Sequential Executor uses SQLite as the default metadata database.

### How to run   

1. Make a directory with the following files and continue the below commands on the same path:   
`docker-compose.yml`   
`.env`   

2. Create the user and initialize docker using the command below
```
docker-compose up airflow-init
```
3. Turn up the docker compose file
```
docker-compose up
```
4. Open "localhost:8081" in your brower and use the credentials as user = admin and password = airflow
