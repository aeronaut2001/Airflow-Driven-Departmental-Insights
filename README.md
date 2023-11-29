# Airflow Driven Departmental Insight
 
 <p align="left"> <img src="https://komarev.com/ghpvc/?username=aeronaut2001&label=Profile%20views&color=0e75b6&style=flat" alt="aeronaut2001" /> </p>
 
[![View My Profile](https://img.shields.io/badge/View-My_Profile-green?logo=GitHub)](https://github.com/aeronaut2001) 
 [![View Repositories](https://img.shields.io/badge/View-My_Repositories-blue?logo=GitHub)](https://github.com/aeronaut2001?tab=repositories)

---

## Department Data Analysis With Apache Hive 🐝
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
<a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> </p>
 
 ---

## 📙 Project Structures :

- [x] **Project Introduction:**
- The project aims to perform data analysis using Apache Hive on a telecom dataset to gain insights into customer behavior, churn, and related factors. Telecom companies often face challenges in retaining customers, making it essential to understand the data for informed decision-making.

- [x] **Problem Statement:**
- The telecom dataset contains information about customers, their services, contracts, and churn status. The goal is to analyze this data to answer various questions and gain actionable insights, including but not limited to:
  - Total number of customers in the dataset.
  - Number of customers who have churned.
  - Distribution of customers based on gender and SeniorCitizen status.
  - Total charge due to churned customers.
  - Churn analysis based on contract type, average monthly charges, tenure, payment methods, and more.
  - Performance optimization with joins when integrating demographic data from another dataset.
  - Advanced analysis, including the distribution of payment methods, churn rates for different InternetService categories, and more.

- [x] **Key Takeaways:**
- At the end of this project, you will have gained valuable experience in using Apache Hive for data analysis, which can be applied to various business scenarios. Some key takeaways from this project include:
  - Proficiency in data loading and exploration in Hive.
  - Ability to perform intermediate and advanced data analysis tasks, such as partitioning and bucketing for better query performance.
  - Understanding the performance implications of different types of joins.
  - Advanced insights into customer behavior, helping the telecom company make data-driven decisions.
  - The ability to identify patterns and factors contributing to churn, enabling proactive customer retention strategies.





























Overview:
The project leverages Apache Airflow to automate the execution of Spark jobs on Google Cloud's Dataproc, ensuring efficient data processing and management.

Key Components:

Airflow DAG: The heart of the project, the Directed Acyclic Graph (DAG) named 'gcp_dataproc_spark_job', defines the workflow. It schedules the execution of Spark jobs on Dataproc, manages cluster creation, job submission, and cluster deletion.

Cluster Configuration: The DAG initiates a Dataproc cluster named 'airflow' with specific configurations tailored for efficient processing. It specifies the number of master and worker nodes, their machine types, and disk configurations.

Dataproc Operators:

DataprocCreateClusterOperator: Initiates the creation of the specified Dataproc cluster based on the provided configuration.
DataprocSubmitPySparkJobOperator: Submits a PySpark job to the created Dataproc cluster, utilizing the specified Python file URI ('gs://data-airflow-input/emp_batch_job.py' in this case).
DataprocDeleteClusterOperator: Ensures the deletion of the Dataproc cluster upon successful completion of the Spark job, maintaining resource efficiency.
Workflow:

Cluster Creation: The DAG triggers the creation of a tailored Dataproc cluster with a defined number of nodes and configurations.

Job Submission: Once the cluster is ready, it submits a PySpark job to the cluster, which fetches and processes data from 'emp_batch_job.py' located in Google Cloud Storage ('gs://data-airflow-input/').

Cluster Deletion: Upon successful job completion, the cluster is automatically deleted, ensuring resource optimization.

Project Impact:

Automation: The project streamlines and automates the entire process, reducing manual intervention and ensuring consistent and reliable data processing.

Scalability: By dynamically creating clusters for specific tasks and removing them afterward, the project allows for scalable and cost-effective data processing.

Learning and Future Improvements:

The project showcases the utilization of Apache Airflow's capabilities in orchestrating data workflows.

Future improvements could include integrating monitoring/logging mechanisms for better job tracking and enhancing cluster configurations based on specific workload requirements.

Conclusion:
This project effectively demonstrates how Airflow can be used to automate Spark job execution on Dataproc, showcasing the power of orchestration in managing data processing workflows efficiently within a cloud environment.










Project Overview:
This project merges Apache Airflow's orchestration capabilities with Google Cloud's Dataproc service to automate Spark job execution for streamlined data processing workflows. The integrated solution ensures efficient handling of tasks while leveraging the cloud environment's scalability.

Key Components:

Airflow DAG:

Named 'gcp_dataproc_spark_job,' the DAG orchestrates the Spark job execution on Dataproc.
It handles the creation, job submission, and deletion of Dataproc clusters.
Cluster Configuration:

The DAG initializes a Dataproc cluster ('airflow') with tailored configurations for optimal performance.
Configurations define node counts, machine types, and disk setups.
Dataproc Operators:

DataprocCreateClusterOperator: Creates the specified Dataproc cluster based on preset configurations.
DataprocSubmitPySparkJobOperator: Submits a PySpark job to the cluster, processing data from 'emp_batch_job.py' in Google Cloud Storage.
DataprocDeleteClusterOperator: Ensures cluster deletion post successful job execution for resource optimization.
Workflow:

Cluster Setup:

The DAG triggers Dataproc cluster creation with predefined settings.
Job Execution:

Upon cluster readiness, it submits a PySpark job to process data from 'emp_batch_job.py' in GCS.
Cluster Cleanup:

After job completion, the DAG deletes the cluster, ensuring resource efficiency.
Project Impact:

Automation: Streamlines tasks, minimizing manual intervention for consistent and reliable data processing.

Scalability: Dynamically creates and removes clusters as needed, offering scalability and cost efficiency.

Learning and Future Improvements:

Demonstrates Airflow's prowess in orchestrating data workflows.
Suggestions for enhancements:
Incorporating monitoring/logging for better job tracking.
Fine-tuning cluster configurations based on workload specifics.
PySpark Script Insights:

The PySpark script provided processes CSV data by:

Initializing a SparkSession for interaction with Spark.
Defining paths for input/output data on Google Cloud Storage (GCS).
Reading CSV files into Spark DataFrames with inferred schema and headers.
Performing data operations like filtering and joining.
Writing the transformed data back to GCS in a CSV file ('joined_output.csv').
Improvement Considerations for the Script:

Incorporating error handling for robustness.
Parameterizing settings for improved flexibility.
Optimizing operations for better performance based on dataset sizes.
Conclusion:

This project showcases how Airflow efficiently manages Spark job execution on Dataproc, highlighting the effectiveness of orchestration in cloud-based data processing workflows.
