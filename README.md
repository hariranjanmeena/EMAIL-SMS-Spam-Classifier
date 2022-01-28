# SMS Spam Classifier

## About

#### [Herokuapp WEB APP](https://spam-sms-email-classifier.herokuapp.com/)

Tried to classify SMS messages as SPAM or NOT SPAM using various ML algorithms. The notebook (SMS Spam Classifier.ipynb) consists of steps to process and explore the dataset, convert messages to vectors and applied ML techniques for the same.

## Dataset
Data is a set of SMS tagged messages that have been collected for SMS Spam research. It contains one set of SMS messages in English of 5,572 messages, tagged according to being ham (legitimate) or spam. The dataset is available here. [link](https://www.kaggle.com/uciml/sms-spam-collection-dataset)

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.

```bash
pip install -r requirements.txt
```

## Exploratory Data Analysis



- I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights from the pivot tables.

![alt text](https://github.com/hariranjanmeena/EMAIL-SMS-Spam-Classifier/blob/8fc55d90a94cd4b987db8adc814c29b78f698066/images/data.PNG)

- Then i created some new features link `num_character`, `num_words`, `num_sentences` 

<img src="https://github.com/hariranjanmeena/EMAIL-SMS-Spam-Classifier/blob/8fc55d90a94cd4b987db8adc814c29b78f698066/images/data2.PNG" width="1000" height="600" />

- Generally count of `num_character` and `num_word` is more in span as compared to ham

![alt text](https://github.com/hariranjanmeena/EMAIL-SMS-Spam-Classifier/blob/8fc55d90a94cd4b987db8adc814c29b78f698066/images/data3.PNG)

- `num_words`, `num_character`, `num_sentences` have high correlation with each other. so we will keep only one of the feature which is num_character because it has high variance with our taget feature which is lable

![alt text](https://github.com/hariranjanmeena/EMAIL-SMS-Spam-Classifier/blob/8fc55d90a94cd4b987db8adc814c29b78f698066/images/heatmap.PNG)


## Wordcloud


![alt text](https://github.com/hariranjanmeena/EMAIL-SMS-Spam-Classifier/blob/4888481602e5675b446f11f4f59c6f29e832f910/images/Aglo's.PNG)

## Model Building 
  
I tried three different models:

![alt text](https://github.com/hariranjanmeena/EMAIL-SMS-Spam-Classifier/blob/4888481602e5675b446f11f4f59c6f29e832f910/images/Aglo's.PNG)

![alt text](https://github.com/hariranjanmeena/EMAIL-SMS-Spam-Classifier/blob/4888481602e5675b446f11f4f59c6f29e832f910/images/alog_graph.PNG)
