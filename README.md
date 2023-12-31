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

- [Apache Spark Downloads](https://spark.apache.org/downloads.html)
    - Choose Spark release: 3.5.0
    - Select package type: "Pre-built for Apache Hadoop 3.3 and later"
    - If these options are not visible, visit the [Spark Release Directory](https://archive.apache.org/dist/spark/)
    - Create the following folder and extract all files there: C:\Spark

### Download Hadoop utilities

- [Hadoop Utilities](https://github.com/cdarlint/winutils/tree/master/hadoop-3.3.5/bin)
    - Create the following folder and extract all files there: C:\hadoop\bin

### Download and install Java Development Kit (JDK)

- [Java Development Kit (JDK) Downloads](https://www.oracle.com/java/technologies/downloads/)
    - Preferably, install in C:\Java

### Download and install Python

- [Python Downloads](https://www.python.org/downloads/)

### Download and install Anaconda project

- [Anaconda Downloads](https://www.anaconda.com/download)

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
- pip install pyspark
- pip install delta-spark

## First steps with Delta Lake

- [Initial setup](https://docs.delta.io/latest/quick-start.html)
- [How to create Delta tables](https://delta.io/blog/2022-10-25-create-delta-lake-tables/)
- [Delta tables read and write](https://docs.delta.io/latest/delta-batch.html#language-python)
- [Delta table project examples (Official)](https://github.com/delta-io/delta/tree/master/examples/python)

## Dataset repositories

- Collection: [DataQuest](https://www.dataquest.io/blog/free-datasets-for-projects/)
- Good option: [Kaggle](https://www.kaggle.com/datasets)
