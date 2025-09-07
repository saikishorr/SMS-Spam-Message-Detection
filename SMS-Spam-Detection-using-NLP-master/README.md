# SMS Spam Detection using Deep Learning in TensorFlow2

This project is about building a spam detection system for SMS messages using deep learning techniques in TensorFlow2. Three different architectures, namely Dense Network, LSTM, and Bi-LSTM, have been used to build the spam detection model. The accuracy of the models is compared and evaluated to select the best one.<br>
### Dataset Link : https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection
The SMS Spam Collection dataset from the UCI Machine Learning Repository is used for this project. The dataset contains 5,574 SMS messages, out of which 4,827 messages are labeled as ham (non-spam) and 747 messages as spam. The dataset is split into 4,000 messages for training and 1,574 messages for testing.<br>
### Steps Involved :
The following steps are involved in the project:<br>

1. Load and Explore the Data: The dataset is loaded into a Pandas DataFrame and explored to get insights into the distribution of ham and spam messages.<br>

2. Prepare Train-Test Data: The messages are tokenized, and their corresponding labels are one-hot encoded. The dataset is split into training and testing sets in the ratio of 80:20.<br>

3. Train the Spam Detection Model: The three models - Dense Network, LSTM, and Bi-LSTM - are trained using the training dataset. The models are evaluated using the validation dataset.<br>

4. Compare and Select the Final Model: The accuracy of the models is compared, and the best-performing model is selected.<br>

5. Use the Final Trained Classifier to Classify New Messages: The final model is used to classify new messages as ham or spam.<br>
### Usage :
To use the SMS spam detection model, follow these steps:<br>

1. Clone the repository: `git clone https://github.com/username/sms-spam-detection.git` <br>
2. Install the required packages: `cd sms-spam-detection`
`pip install -r requirements.txt` <br>
3. Download the dataset from the UCI Machine Learning Repository and place it in the data directory: `mkdir data`
`wget https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection -O data/spam.csv`<br>
4. Run the .pynb script to train the models and select the best one <br>
5. Run the streamlit app as :  `streamlit run app.py`<br>

### Accuracy of the Models :
The accuracy of the models is as follows: <br>

Dense Network - 98.5%<br>
SVM - 97.6%<br>
Bi-LSTM - 98.8%<br>
LSTM - 98.6%<br>
### Streamlit App :
A Streamlit app has been created to showcase the working of the final model. The app takes a message as input and predicts whether it is ham or spam. The app can be accessed using the following link:<br>

https://deepankarvarma-sms-spam-detection-using-nlp-app-atp0na.streamlit.app/
<br>
### Conclusion :
In this project, we have built a spam detection system for SMS messages using deep learning techniques in TensorFlow2. Three different architectures have been used to build the spam detection model. The Bi-LSTM model performed the best, with an accuracy of 98.8%. The final model has been deployed as a Streamlit app to showcase its working.
