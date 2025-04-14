##**Project Overview:** Language Detection through Text
This project implements a multilingual language detection system using both machine learning and deep learning models. It compares the performance of four different model combinations for identifying languages from text input. The dataset used includes over 10,000 text samples across 17 languages.

##**Source Code Structure and File Descriptions**
**language_detection.py-**
This is the main Python script. It contains all the logic for loading the dataset, preprocessing text data, building and training the models, and making predictions. It also prints evaluation metrics like Accuracy, F1 Score, and Precision.

**Language Detection.csv-**
This is the dataset file. It contains labeled examples of text and their corresponding language, used for training and testing the models.

**README.md-**
This file provides documentation of the project, including setup instructions, how to run the script, and details about the model architecture and evaluation.

##**Setup Instructions-**
Before running the code, make sure the following libraries are installed. You can run this in your terminal or Colab:
bash-pip install pandas numpy scikit-learn tensorflow
**How to Run the Project**
You can run the project using any Python 3.6+ environment (like Anaconda, local Python setup, or Google Colab).

**Step 1:** Run the Training and Testing Script
In your Python environment or terminal, run the main script:
**python language_detection.py**
This will:
-Load and preprocess the dataset
-Train all four models
-Evaluate each model
-Display accuracy, F1 score, and precision
-Print a comparison of all models

**Step 2:** Test with Custom Input
At the end of the script, there's a prediction section. You can modify the input line to test with your own sentence:
**predict_language("Bonjour, comment allez-vous aujourd'hui?")**
The output will show the predicted language for each model.

##**Models Included**
The script includes the following four models:
-Naive Bayes + N-Gram
-CNN + N-Gram
-Naive Bayes + TF-IDF
-CNN + TF-IDF
Each model is trained on the same dataset and evaluated using the same metrics for a fair comparison.

Output (Summary Table)

Model Performance Comparison:
                             Model        Accuracy   F1 Score   Precision
0         Naive Bayes + N-Gram         0.9501      0.9512     0.9581
1         CNN + N-Gram                 0.9589      0.9597     0.9632
2         Naive Bayes + TF-IDF         0.9521      0.9529     0.9592
3         CNN + TF-IDF                 0.9608      0.9615     0.9638

##**Requirements**
Make sure the following are installed:
-Python 3.6 or later
-pandas
-numpy
-scikit-learn
-tensorflow or keras

