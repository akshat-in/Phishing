# Phishing URL Detection

![image](https://github.com/srijansingh08/Phishing-URL-Detection/assets/65160855/c34c34d4-537c-4543-b684-e0eeedd037f6)

![image](https://github.com/srijansingh08/Phishing-URL-Detection/assets/65160855/935fbed3-7533-4b86-a45c-2fdb61371562)


## Table of Content

- [Introduction](#introduction)
- [Installation](#installation)
- [Directory Tree](#directory-tree)
- [Result](#result)
- [Conclusion](#conclusion)

## Introduction

The Internet has become an indispensable part of our life, However, It also has provided opportunities to anonymously perform malicious activities like Phishing. Phishers try to deceive their victims by social engineering or creating mockup websites to steal information such as account ID, username, password from individuals and organizations. Although many methods have been proposed to detect phishing websites, Phishers have evolved their methods to escape from these detection methods. One of the most successful methods for detecting these malicious activities is Machine Learning. This is because most Phishing attacks have some common characteristics which can be identified by machine learning methods.

## Installation

The Code is written in Python 3.11.2. If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository:

```bash
pip install -r requirements.txt
```

## Directory Tree

```
├── pickle
│   ├── model.pkl
├── static
│   ├── styles.css
├── templates
│   ├── index.html
├── Phishing URL Detection.ipynb
├── Procfile
├── README.md
├── app.py
├── feature.py
├── phishing.csv
├── requirements.txt


```

## Technologies Used

![](https://forthebadge.com/images/badges/made-with-python.svg)

[<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/3/31/NumPy_logo_2020.svg" width=200>](https://numpy.org/doc/) [<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/e/ed/Pandas_logo.svg" width=200>](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html)
[<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/8/84/Matplotlib_icon.svg" width=100>](https://matplotlib.org/)
[<img target="_blank" src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" width=200>](https://scikit-learn.org/stable/)
[<img target="_blank" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcScq-xocLctL07Jy0tpR_p9w0Q42_rK1aAkNfW6sm3ucjFKWML39aaJPgdhadyCnEiK7vw&usqp=CAU" width=200>](https://flask.palletsprojects.com/en/2.0.x/)

## Result

Accuracy of various model used for URL detection
<br>

<br>

    ML Model	Accuracy	f1_score	Recall	Precision

0 Gradient Boosting Classifier 0.974 0.977 0.994 0.986

1 CatBoost Classifier 0.972 0.975 0.994 0.989

2 Support Vector Machine 0.964 0.968 0.980 0.965

3 Random Forest 0.964 0.968 0.994 0.989

4 Decision Tree 0.960 0.964 0.991 0.993

5 K-Nearest Neighbors 0.956 0.961 0.991 0.989

6 Logistic Regression 0.934 0.941 0.943 0.927

7 Naive Bayes Classifier 0.605 0.454 0.292 0.997

8 XGBoost Classifier 0.549 0.544 0.987 0.987

9 Multi-layer Perceptron 0.547 0.541 0.988 0.988


Feature importance for Phishing URL Detection
<br><br>
![image](https://user-images.githubusercontent.com/79131292/144603941-19044aae-7d7b-4e9a-88a8-6adfd8626f77.png)

## Conclusion

1. The final take away form this project is to explore various machine learning models, perform Exploratory Data Analysis on phishing dataset and understanding their features.
2. Creating this notebook helped me to learn a lot about the features affecting the models to detect whether URL is safe or not, also I came to know how to tuned model and how they affect the model performance.
3. The final conclusion on the Phishing dataset is that the some feature like "HTTTPS", "AnchorURL", "WebsiteTraffic" have more importance to classify URL is phishing URL or not.
4. Gradient Boosting Classifier currectly classify URL upto 97.4% respective classes and hence reduces the chance of malicious attachments.
