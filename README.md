# Automated Classification of Inappropriate Textual Content


## Introduction
This project aims to develop an automated content moderation system capable of classifying textual content as appropriate or inappropriate for public display. The system leverages machine learning models and natural language processing techniques to analyze textual data and provide classification results in real-time.

## Files Included
1. 'Data_Preprocessing.ipynb': Jupyter notebook for loading and preprocessing the dataset ('hate_offensive_data.csv') to create a new CSV file ('preprocessed_data.csv').
2. 'LSTM.ipynb': Jupyter notebook for training and evaluating the LSTM model for text classification using the preprocessed data.
3. 'BERT.ipynb': Jupyter notebook for training and evaluating the BERT model for text classification using the preprocessed data.
4. 'requirements.txt': File listing the Python libraries required to be installed before executing the code.
5. 'Flask_app/main.py': Python file for the Flask application. This file handles text and image inputs through a web browser, loads the trained BERT model, and accesses the Google Cloud Vision API for text extraction from images.
6. 'Flask_app/templates/index5.html': HTML page for the Flask application.
7. 'Flask_app/app.yaml' : Configuration file required for deploying the Flask application on Google App Engine.

## Steps to Simulate the Project
1. Download the zip file and unzip it.
2. Install the required Python libraries listed in 'requirements.txt': pip install -r requirements.txt
3. Run 'Data_Preprocessing.ipynb' to preprocess the dataset and generate the 'preprocessed_data.csv' file.
4. Open and run 'LSTM.ipynb' to train and evaluate the LSTM model for text classification using the preprocessed data.
5. Open and run 'BERT.ipynb' to train and evaluate the BERT model for text classification using the preprocessed data.
6. Navigate to the 'Flask_app' directory and run the Flask application by executing the following command: python main.py
7. Access the Flask application through a web browser by visiting 'http://localhost:5000/'. You can input text or upload images to receive classification results based on the content provided.

WebApp Link: https://moderator-415722.ue.r.appspot.com/ (It might take around 30-40 seconds to load)

Note: 
Trained model (BERT) files are not included in the repository and need to be trained separately using the provided notebooks. 
BERT training may take time. We had used Google Colab to train it faster. 
Also, Please change the file locations in the python files accordingly.




