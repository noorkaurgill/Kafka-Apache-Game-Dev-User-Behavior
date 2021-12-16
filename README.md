# Understanding User Behavior

## Project Summary:
Through this project, we function as data scientists at a game development company where latest mobile game has two events you're interested in tracking: `buy a sword` & `join guild` (each having metadata characteristics). We are tasked with instrumenting the API server to log events to Kafka as well as assembling a data pipeline to catch these events by using Spark streaming to filter, selecting event types from Kafka, and landing them into HDFS/parquet to make them available for analysis using Presto. Also, we must use Apache Bench to generate test data for the pipeline and produce an analytics report with pipeline description and basic event analysis. 

## Directory:
1. [Project_Directions.md](https://github.com/mids-w205-schioberg/project-3-noorkaurgill/blob/assignment/Project_Directions.md)
    - Given project directions
    
2. [docker-compose.yml](https://github.com/mids-w205-schioberg/project-3-noorkaurgill/blob/assignment/docker-compose.yml)
    - YML file used to spin up the cluster

3. [game_api.py](https://github.com/mids-w205-schioberg/project-3-noorkaurgill/blob/assignment/game_api.py)
    - Where the API server is instrumented with 2 events (purchase_a_sword and join_a_guild)

4. [purchase_sword_stream_and_hive.py](https://github.com/mids-w205-schioberg/project-3-noorkaurgill/blob/assignment/purchase_sword_stream_and_hive.py)
    - Allows for filtering, writing the metadata to Hive python script, and storing to HDFS for the purchasing sword event
    
   [join_guild_stream_and_hive.py](https://github.com/mids-w205-schioberg/project-3-noorkaurgill/blob/assignment/join_guild_stream_and_hive.py)
   - Allows for filtering, writing the metadata to Hive python script, and storing to HDFS for the joining guild event

5. [Project_03.ipynb](https://github.com/mids-w205-schioberg/project-3-noorkaurgill/blob/assignment/Project_3.ipynb)
    - Report in the form of a Jupyter notebook that describes queries and spark SQL to answer selected business questions
    - Goes into further details to explain code and steps in pipeline creation

6. [README.md](https://github.com/mids-w205-schioberg/project-3-noorkaurgill/blob/assignment/README.md)
    - (This file) lays out basic overview and directory with descriptions of repository files

7. [Images Folder](https://github.com/mids-w205-schioberg/project-3-noorkaurgill/tree/assignment/Images)
    - Contains images that represent outputs of the commands discussed on the report (Project_03.ipynb)
    
