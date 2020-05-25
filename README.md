# Disaster Response Pipeline Project

<h2>Project Components</h2>
There are three components you'll need to complete for this project.

<h4>1. ETL Pipeline</h4>
In a Python script, process_data.py, write a data cleaning pipeline that:

-Loads the messages and categories datasets

-Merges the two datasets

-Cleans the data

-Stores it in a SQLite database


<h4>2. ML Pipeline</h4>
In a Python script, train_classifier.py, write a machine learning pipeline that:

-Loads data from the SQLite database

-Splits the dataset into training and test sets

-Builds a text processing and machine learning pipeline

-Trains and tunes a model using GridSearchCV

-Outputs results on the test set

-Exports the final model as a pickle file


<h4>3. Flask Web App</h4>
We are providing much of the flask web app for you, but feel free to add extra features depending on your knowledge of flask, html, css and javascript. For this part, you'll need to:

-Modify file paths for database and model as needed

-Add data visualizations using Plotly in the web app. One example is provided for you

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/
