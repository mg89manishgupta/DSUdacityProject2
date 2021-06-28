# Disaster Response Pipeline Project

### Installation

The following Python packages are required to be installed : pandas, numpy, re, pickle, nltk, flask, json, plotly, sklearn, sqlalchemy, sys, warnings.

### Project Overview

The project is written to execute a web app which can help in emergency operations during a disaster by exploting a response system to classify a disaster text messages into several categories which then can be transmited to the responsible entity.
The app built to have an ML model to categorize every message received

### File Description:

1. process_data.py: This python script takes csv files containing message data and message categories and then creates a SQL database
2. train_classifier.py: This code trains the ML model with the SQL data base
3. run.py - python script used to initiate the web app

### Instructions:

1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        'python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db'
    - To run ML pipeline that trains classifier and saves
        'python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl'

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

### Licensing, Authors, Acknowledgements

The project has been completed as part of the Udacity Data Scientist Nanodegree.