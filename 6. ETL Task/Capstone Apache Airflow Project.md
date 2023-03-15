# Apache Airflow Workflow for Capstone project

## Start Airflow

```
start_airflow
```
## Create a dir in the following folder /home/projects/airflow/dags/
```
mkdir /capstone
```
## Download the source file in the capstone dir
```
wget https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0321EN-SkillsNetwork/ETL/accesslog.txt
```

## create a python DAG file called process_web_log.py
```

```
## Once the DAG file is ready, submit the DAG to airflow

### Go back to the projects folder
```
cd .. 
```

### Copy the DAG file from the project folder to the /airflow/dags directory
```
sudo cp process_web_log.py /home/projects/airflow/dags
```

### Change the execution mode of the .py file in the directory
```
sudo chmod +x process_web_log.py
```

### You might also need to change the permission settings also for the capstone directory
```
sudo chmod 777 /home/project/airflow/dags/capstone
```

### Check the airflow dag list
```
airflow dags list
```

### Unpause the submitted DAG
```
airflow unpause process_web_log
```

