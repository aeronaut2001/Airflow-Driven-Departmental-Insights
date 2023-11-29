# Airflow Driven Departmental Insight
 
 <p align="left"> <img src="https://komarev.com/ghpvc/?username=aeronaut2001&label=Profile%20views&color=0e75b6&style=flat" alt="aeronaut2001" /> </p>
 
[![View My Profile](https://img.shields.io/badge/View-My_Profile-green?logo=GitHub)](https://github.com/aeronaut2001) 
 [![View Repositories](https://img.shields.io/badge/View-My_Repositories-blue?logo=GitHub)](https://github.com/aeronaut2001?tab=repositories)

---

## Department Data Analysis With Apache Airflow and Spark
📝 Gain the skills 
---

 <h3 align="left">Languages and Tools:</h3>

<p align="left"> Cloud: </p>

<a href="https://cloud.google.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="40" height="40"/> </a> </p>

<p align="left"> Version Control System: </p>

 <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> </p>

<p align="left"> Programming Language - PYTHON: </p>
    <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> 

<p align="left"> BIG DATA TOOL AND SOFTWARES: </p> 
  <a href="https://hadoop.apache.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/apache_hadoop/apache_hadoop-icon.svg" alt="hadoop" width="40" height="40"/> </a> 
  <a href="https://hive.apache.org" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/b/bb/Apache_Hive_logo.svg" alt="Apache Hive" width="40" height="40"/> </a> 
  <a href="https://spark.apache.org" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/f/f3/Apache_Spark_logo.svg" alt="Apache Spark" width="40" height="40"/> </a> 
<a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> </p>

<p align="left"> WORKFLOW MANAGEMENT: </p> 
<a href="https://airflow.apache.org" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/d/de/AirflowLogo.png" alt="Apache Airflow" width="40" height="40"/> </a></p>
 
 ---

## 📙 Project Structures :

- [x] **Project Introduction:**
- The project leverages Apache Airflow to automate the execution of Spark jobs on Google Cloud's Dataproc, ensuring efficient data processing and management.
- [x] **Cluster Configuration:**
- The DAG initializes a Dataproc cluster ('airflow') with tailored configurations for optimal performance.Configurations define node counts, machine types, and disk setups.
- [x] **Dataproc Operators:**
- DataprocCreateClusterOperator: Creates the specified Dataproc cluster based on preset configurations.
- DataprocSubmitPySparkJobOperator: Submits a PySpark job to the cluster, processing data from 'emp_batch_job.py' in Google Cloud Storage.
- DataprocDeleteClusterOperator: Ensures cluster deletion post successful job execution for resource optimization.
- [x] **Workflow:**
- Cluster Setup:
  - The DAG triggers Dataproc cluster creation with predefined settings.
- Job Execution:
  - Upon cluster readiness, it submits a PySpark job to process data from 'emp_batch_job.py' in GCS.
- Cluster Cleanup
  - After job completion, the DAG deletes the cluster, ensuring resource efficiency.
- Project Impact:
  - Automation: Streamlines tasks, minimizing manual intervention for consistent and reliable data processing.
- Scalability:
  - Dynamically creates and removes clusters as needed, offering scalability and cost efficiency.
- Learning and Future Improvements:
  - Demonstrates Airflow's prowess in orchestrating data workflows.
- [x]**The PySpark script provided processes CSV data by:**
  - Initializing a SparkSession for interaction with Spark.
  - Defining paths for input/output data on Google Cloud Storage (GCS).
  - Reading CSV files into Spark DataFrames with inferred schema and headers.
  - Performing data operations like filtering and joining.
  - Writing the transformed data back to GCS in a CSV file ('joined_output.csv').


- [x] **Key Takeaways:**
- This project effectively demonstrates how Airflow can be used to automate Spark job execution on Dataproc, showcasing the power of orchestration in managing data processing workflows efficiently within a cloud environment.




























