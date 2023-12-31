# Project

The objective of this project is to establish a local environment for exploring the capabilities of Spark combined with the Delta Lake engine, without any cost.

## Directories

The folder structure includes:
- Delta Lake  - This path is designated for writing Delta Tables.
- Notebooks   - Python Notebooks are developed in this path.
- Power BI    - This directory hosts a small Power BI project for exploring data in local Delta Tables.
- Setup Files - Various datasets are stored in this directory.

## Setup Files

### Download Apache Spark with Hadoop

- <a href="https://spark.apache.org/downloads.html" target="_blank">Apache Spark Downloads</a>
  - Choose Spark release: 3.5.0
  - Select package type: "Pre-built for Apache Hadoop 3.3 and later"
  - If these options are not visible, visit the <a href="https://archive.apache.org/dist/spark/" target="_blank">Spark Release Directory</a>
  - Create the following folder and extract all files there: C:\Spark

### Download Hadoop utilities

- <a href="https://github.com/cdarlint/winutils/tree/master/hadoop-3.3.5/bin" target="_blank">Hadoop Utilities</a>
  - Create the following folder and extract all files there: C:\hadoop\bin

### Download and install Java Development Kit (JDK)

- <a href="https://www.oracle.com/java/technologies/downloads/" target="_blank">Java Development Kit (JDK) Downloads</a>
  - Preferably, install in C:\Java

### Download and install Python

- <a href="https://www.python.org/downloads/" target="_blank">Python Downloads</a>

### Download and install Anaconda project

- <a href="https://www.anaconda.com/download" target="_blank">Anaconda Downloads</a>

## Environment variables

- Open "Environment Variables" in Windows Settings
  - Add new user variables:
    - Java
      - Name: JAVA_HOME
      - Path: Browse until the "jdk" folder in the Java installation directory, e.g., "C:\Program Files\Java\jdk-21" or "C:\Java\jdk-21"
    - Python
      - Name: PYSPARK_HOME
      - Path: Browse until the Python file (python.exe) in the installation directory, e.g., "C:\Users\<user>\AppData\Local\Programs\Python\Python312\python.exe"
    - Hadoop
      - Name: HADOOP_HOME
      - Path: Browse until the Hadoop files directory, e.g., "C:\hadoop"
    - Spark
      - Name: SPARK_HOME
      - Path: Browse until the Spark files directory, e.g., "C:\Spark\spark-3.5.0-bin-hadoop3"
  - Add the path for the "bin" directories to System Variables:
    - Edit the variable "path" and add, by clicking "New," the following:
      - %JAVA_HOME%\bin
      - %SPARK_HOME%\bin
      - %HADOOP_HOME%\bin

## Important Python Wheels

Open the command prompt and run the following:
- <a href="https://pypi.org/project/pyspark/" target="_blank">pip install pyspark</a>
- <a href="https://pypi.org/project/delta-spark/" target="_blank">pip install delta-spark</a>

## First steps with Delta Lake

- <a href="https://docs.delta.io/latest/quick-start.html" target="_blank">Initial setup</a>
- <a href="https://delta.io/blog/2022-10-25-create-delta-lake-tables/" target="_blank">How to create Delta tables</a>
- <a href="https://docs.delta.io/latest/delta-batch.html#language-python" target="_blank">Delta tables read and write</a>
- <a href="https://github.com/delta-io/delta/tree/master/examples/python" target="_blank">Delta table project examples (Official)</a>

## Dataset repositories

- Collection: <a href="https://www.dataquest.io/blog/free-datasets-for-projects/" target="_blank">DataQuest</a>
- Good option: <a href="https://www.kaggle.com/datasets" target="_blank">Kaggle</a>
