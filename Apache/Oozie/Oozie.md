# Oozie

## What is Oozie?
* Apache Oozie is a scheduler system to run and manage Hadoop jobs in a distributed environment.
* Allows jobs to be run in sequential or parallel order.
* It is an Open Source Java Web-Application responsible for triggering the workflow actions, which in turn uses the Hadoop execution engine to actually execute the task.
* Hadoop Developers use Oozie for performing ETL operations on data in a sequential order and saving the output in a specified format (Avro, ORC, etc.) in HDFS.

## Types of Jobs in Oozie?
* **Workflow Jobs** − Represented as Directed Acyclic Graphs (DAGs) to specify a sequence of actions to be executed.
* **Coordinator Jobs** − Consist of workflow jobs triggered by time and data availability.
* **Oozie Bundle** − Package of multiple coordinator and workflow jobs.

## Oozie Workflow
* Sequence of actions arranged in a control dependency DAG (Direct Acyclic Graph).
* The actions are in controlled dependency as the next action can only run as per the output of current action. Subsequent actions are dependent on its previous action. A workflow action can be a Hive action, Pig action, Java action, Shell action, etc. There can be decision trees to decide how and on which condition a job should run.
* A fork is used to run multiple jobs in parallel
* Oozie workflows can be parameterized (variables like ${nameNode} can be passed within the workflow definition). These parameters come from a configuration file called as property file.


## References
https://www.tutorialspoint.com/apache_oozie/index.htm