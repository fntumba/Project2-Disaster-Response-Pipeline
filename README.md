# Disaster Response Pipeline Project

### Project Motivation
In this project, you'll find a data set containing real messages that were sent during disaster events. You will find a code for a machine learning pipeline to categorize those events so that you can send the messages to an appropriate disaster relief agency.

This project include a web app where an emergency worker can input a new message and get classification results in several categories. The web app will also display visualizations of the data.


### Installation
There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3.*.

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data_new.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier_new.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

### Files descriptions
- app
  
    | - template

        | | - master.html  # main page of web app

        | | - go.html  # classification result page of web app

    |- run.py  # Flask file that runs app

- data
  
    | - disaster_categories.csv  # data to process 

    | - disaster_messages.csv  # data to process

    | - process_data.py

    | - InsertDatabaseName.db   # database to save clean data to


- models
  
    |- train_classifier.py

    |- classifier.pkl  # saved model 


- README.md
