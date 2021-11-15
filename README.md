<h1> Fake News Detection - ML IA 2 </h1>
The team members are: 
<ul>
  <li>Purvi Harniya, 1814023 </li>
  <li>Neelay Jagani, 1814024</li>
  <li>Esha Gupta,1814025</li>
</ul>

---

<h2>INTRODUCTION</h2>

Data has been increasing at an unprecedented range in an exponential manner and is producing 2.7 quintillion bytes of data everyday.

The definition of fake news is information that pushes people down the wrong road. Fake news is spreading like wildfire these days, and people are sharing it without confirming it. This is frequently done to promote or impose specific views, and it is frequently accomplished through political agendas.

As a result, it is vital to recognise fake news. 

---

<h2>PROBLEM DEFINITION </h2>

Fake News have become more prevalent in recent years and with great amount of dynamism in internet and social media, differentiating between facts and opinions, relating to commercial or political upheavals has become more difficult than ever.

Fake information is purposely or unintentionally spread throughout the internet. The massive dissemination of fake news has left an indelible mark on people and culture.

We use various NLP and preprocessing methodologies like tokenization, stop words removal, lemmatization, stemming and machine learning classification algorithms - logistic regression, pac, ada, naive bayes, svm, random forest, xgboost, decision trees and rnn, to build a model that differentiates between fake news and real news and also analyze the performance of these various classification methodologies to choose the best classifier on out dataset.

---

<h2>IMPLEMENTATION DETAILS</h2>

The ISOT Fake news dataset was downloaded from https://www.uvic.ca/ecs/ece/isot/datasets/index.php. 

![image](https://drive.google.com/uc?export=view&id=1GLrh_FDq4haS9Cic54zC2adUfaujNzC3) <br>
![image](https://drive.google.com/uc?export=view&id=1HfWSHpAYcYvQA1Dg6OtCzgiyLMOzPB1t)


A comparison of various classification algorithms to determine the best for our dataset.
The results are as follows: <br>

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Models</th>
      <th>Accuracy</th>
      <th>Precision</th>
      <th>F1 Score</th>
      <th>Recall</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>Logstic Regression</td>
      <td>0.987973</td>
      <td>0.986926</td>
      <td>0.987387</td>
      <td>0.987848</td>
    </tr>
    <tr>
      <th>2</th>
      <td>ADA</td>
      <td>0.988241</td>
      <td>0.987661</td>
      <td>0.987661</td>
      <td>0.987661</td>
    </tr>
    <tr>
      <th>3</th>
      <td>PAC</td>
      <td>0.995724</td>
      <td>0.994958</td>
      <td>0.995516</td>
      <td>0.996074</td>
    </tr>
    <tr>
      <th>4</th>
      <td>XGB</td>
      <td>0.990468</td>
      <td>0.994342</td>
      <td>0.989954</td>
      <td>0.985605</td>
    </tr>
    <tr>
      <th>5</th>
      <td>RF</td>
      <td>0.984677</td>
      <td>0.986835</td>
      <td>0.983874</td>
      <td>0.980931</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Naive Bayes</td>
      <td>0.952339</td>
      <td>0.951087</td>
      <td>0.949930</td>
      <td>0.948775</td>
    </tr>
    <tr>
      <th>7</th>
      <td>SVM</td>
      <td>0.994833</td>
      <td>0.993287</td>
      <td>0.994586</td>
      <td>0.995887</td>
    </tr>
    <tr>
      <th>8</th>
      <td>DT</td>
      <td>0.985835</td>
      <td>0.986684</td>
      <td>0.985114</td>
      <td>0.983548</td>
    </tr>
    <tr>
      <th>9</th>
      <td>RNN</td>
      <td>0.992428</td>
      <td>0.994877</td>
      <td>0.992104</td>
      <td>0.989347</td>
    </tr>
  </tbody>
</table>
<br>

![image](https://drive.google.com/uc?export=view&id=1c8ZJ83ROOYwgwzgf9tboHEgLoIX0J8Yg) <br>
![image](https://drive.google.com/uc?export=view&id=1bkPVQDVXXoxCQxXLBBFsibz0SYWmFVd3) <br>

---
<h2> Conclusion </h2>

We downloaded the ISOT dataset from https://www.uvic.ca/ecs/ece/isot/datasets/index.php and uploaded it to our drive, and then loaded it and preprocessed it using various NLP algorithms like tokenization, stop words removal, lemmatization and stemming. We vectorized the text documents using count vectorizer and tf-idf vectorizer. After preprocessing, we split the data into testing and training and we built nine models using nine different classification algorithms and used the predictions to calculate the performance metrics. The details of each are given below:

![image](https://drive.google.com/uc?export=view&id=1j-NHuvGKlop7YiY6dbkUoewRTkZoXw-x) <br>

From the ROC curve and the bar plot which compares the performance of all the models, we conclude that the SVM (accuracy-99.48%, precision - 99.33%, f1 score-99.46%, recall-99.59%) is the best algorithm on our ISOT dataset for the task of fake news detection and classification. 

The main notebook file is 'Group6_Code_ML_IA2_Implementation.ipynb' - https://github.com/Purviharniya/Fake-news-detection/blob/master/Group6_Code_ML_IA2_Implementation.ipynb <br>
The dataset is available in the dataset folder -  https://github.com/Purviharniya/Fake-news-detection/tree/master/dataset <br>
The notebook file's pdf is available at - https://github.com/Purviharniya/Fake-news-detection/blob/master/Group6_CodePDF_ML_IA2.pdf <br>
The ppt is available at - https://github.com/Purviharniya/Fake-news-detection/blob/master/Group6_PPT_ML_IA2.pptx  <br>
The summary document is available at - https://github.com/Purviharniya/Fake-news-detection/blob/master/Group6_Document_FakeNewsDetection_ML_IA2_EXP8.docx <br>
The screen cast is available at - https://github.com/Purviharniya/Fake-news-detection/blob/master/Group6_Screencast_ML_IA2.mp4 <br>
The research paper for IA1 - https://github.com/Purviharniya/Fake-news-detection/blob/master/Group6_Reasearch%20Paper_ML_IA.pdf <br>

---
