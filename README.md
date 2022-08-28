## About The Project

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming application. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the application, as well as a directory with JSON meta-data on the songs in their application.

They'd like a data engineer to create a Apache Cassandra database which can create queries on song play data to answer the questions and make meaningful insights. The role of this project is to create a database schema and ETL pipeline for this analysis. 

### Project Description

In this project, we will carry out data modeling with Apache Cassandra and complete an ETL pipeline using Python. The ETL pipeline extracts data from a set of CSV files within a directory to create a streamlined CSV file to model and insert data into Apache Cassandra tables. We will create tables based on specific queries, leveraging partition keys and clustering columns.


### Dataset

#### Event Dataset

Event dataset is a collection of CSV files containing the information of user activity across a period of time.  Each file in the dataset contains the information regarding the song played, user information and other attributes . 

List of available data columns :

```
artist, auth, firstName, gender, itemInSession, lastName, length, level, location, method, page, registration, sessionId, song, status, ts, userId
```

## Project Structure

Files in this repository:

|     File / Folder      |                         Description                          |
| :--------------------: | :----------------------------------------------------------: |
|       event_data       | Folder at the root of the project, where project data is stored |
|         images         |  Folder at the root of the project, where images are stored  |
| event_datafile_new.csv | Contains the data after merging the CSV files at `event_data` |
|    Project2.ipynb     | iPython notebook containing the ETL pipeline steps and codes|
|         README         |                         Readme file                          |



<!-- GETTING STARTED -->

## Getting Started

Clone the repository into a local machine using

```sh
git clone https://github.com/ObinnaIheanachor/Data-Engineering-ND-P2-Sparkify
```

### Prerequisites

These are the prerequisites to run the program.

* python 3.7 or above
* Apache Cassandra
* cassandra python library

### How to run

Follow the steps to extract and load the data into the data model.

1. Run `Project 2.ipynb` iPython notebook
2. Run Part 1 to create `event_datafile_new.csv` 
3. Run Part 2 to Extract and Load data inti tables

4. Confirm data has been loaded by executing `SELECT` queries
