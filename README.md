# Project

The goal of this project is to create a environment in local machine to explore the Spark combined with Delta Lake engine capabilities for free.

## Directories

The structure of the folders is:
- Delta Lake  - Path where the Delta Tables will be writen
- Notebooks   - Path where the Python Notebooks will be developed
- Power BI    - Small project in Power BI to explore the data in local Delta Tables
- Setup Files - All the files needed to setup the project

## Setup Files

- Download Apache Spark with Hadoop
    - https://spark.apache.org/downloads.html
        - Choose a Spark release: 3.5.0
        - Choose a package type:  "Pre-built for Apache Hadoop 3.3 and later"
        - If these options aren't appearing, go to the Spark Release Directory: https://archive.apache.org/dist/spark/
        - Create the following folder and extract all the files there: C:\Spark

- Download Hadoop utilities
    - https://github.com/cdarlint/winutils/tree/master/hadoop-3.3.5/bin
        - Create the following folder and extract all the files there: C:\hadoop\bin

- Download and install Java Development Kit ( JDK )
    - https://www.oracle.com/java/technologies/downloads/
    - 
    
- Download and install Python
    - https://www.python.org/downloads/

- Download and install Anaconda project
    - https://www.anaconda.com/download

## Environment variables


## First steps with Delta Lake

- Initial setup: https://delta.io/learn/getting-started/
- How to create delta tables: https://delta.io/blog/2022-10-25-create-delta-lake-tables/
- Delta tables read and write: https://docs.delta.io/latest/delta-batch.html#language-python
- Delta table project examples ( Official ): https://github.com/delta-io/delta/tree/master/examples/python

## Dataset repositories

- Collection:  https://www.dataquest.io/blog/free-datasets-for-projects/
- Good option: https://www.kaggle.com/datasets