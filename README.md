# Disaster Response Pipeline Project
This Project is part of Data Science Nanodegree Program by [Udacity](https://classroom.udacity.com/nanodegrees/nd025) in collaboration with [Figure Eight](https://appen.com/). The dataset contains pre-labelled tweet and messages from real-life disaster events. The project aim is to build a Natural Language Processing (NLP) model to categorize messages on a real time basis.

# Table of Contents:

1.Project Description

2.Installations

3.File Descriptions

4.Instructions

5.Results and Screenshots

6.Licensing, Authors, Acknowledgements


# Project Description:
This Project is one of the Data Science Nanodegree Program of [Udacity](https://classroom.udacity.com/nanodegrees/nd025). The initial dataset contains pre-labelled tweet and messages from real-life disaster situations that was provided by [Figure Eight](https://appen.com/). By classifying these messages, we can allow these messages to be sent to the appropriate disaster relief agency. This project will involve the building of a basic ETL and Machine Learning pipeline to facilitate the task. 

The Project is divided in the following Sections:

1.Processing Data, ETL Pipeline for extracting data from source, cleaning data and saving them in a proper database structure.

2.Machine Learning Pipeline for training a model to be able to classify text message in categories.

3.Web App for showing model results in real time.

# Installations:

Must be runing fine with Python 3 and above with libraries of numpy, pandas, sqlalchemy, re, NLTK, pickle, Sklearn, plotly and flask libraries.

# File Descriptions:

1.App Folder: This folder contains 1 folder named "templates" and 1 file name "run.py" 

    i.Templates folder: This folder contains 2 files "go.html" and "master.html" both the files contains webapp styling code.
    
    ii.run.py: This file cotains code to run the webapp.
    
2.Data Folder: This folder contains "DisasterResponse.db", "disaster_categories.csv", "disaster_messages.csv" and "process_data.py" for data cleaning and transfering.

3.Models Folder: This folder contains a "train_classifier.py" and a pickle file "classifier.pkl" which is created after running "train_classifier.py".

4.Preparation Files used for project building.

5.Screenshots of webapp.

# Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

# Results and Screenshots:

The below screenshots are the result of running the webapp.

![Screenshot1](https://user-images.githubusercontent.com/25797072/122058608-6c2f5180-ce09-11eb-9366-e7aa7d280ba1.PNG)

![Screenshot2](https://user-images.githubusercontent.com/25797072/122058631-718c9c00-ce09-11eb-8c0d-719da0f97c04.PNG)

Once after specifing the disaster in the search box and clicking the classify message button in webapp gives all the related response centres with highlighted text.

![Screenshot3](https://user-images.githubusercontent.com/25797072/122058640-74878c80-ce09-11eb-86ea-d0257061500d.PNG)



# Licensing, Authors, Acknowledgements

Thanks to [Udacity](https://classroom.udacity.com/nanodegrees/nd025) and [Figure Eight](https://appen.com/) for providing such a insightful nanodegree program and for providing dataset,and a big thanks to stackoverflow for clearing my doubts.
