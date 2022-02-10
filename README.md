# toxic_comment_classification

## Requirements
```
numpy==1.19.0
scipy
seaborn==0.11.1
matplotlib
matplotlib-venn==0.11.6
prettytable==2.4.0
plotly==5.4.0
sklearn==0.0
nltk==3.6.5
tensorflow==2.7.0
```

[Jigsaw toxic comment classification](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge) is a challenge to detect 
different levels of toxicity like Threats, Obscenity, Insults & Identitiy Hates. 

*Disclaimer: the dataset contains text that may be considered profane, vulgar or offensive.*

## Exploratory Data Analysis

Train Data - 159571 x 8
Test Data - 153164 x 2

+----------------------+---------+
|       Field 1        | Field 2 |
+----------------------+---------+
|    Total Comments    |  159571 |
| Total clean comments |  143346 |
|     Total labels     |  35098  |
+----------------------+---------+

Comments per Label
toxic            15294
severe_toxic      1595
obscene           8449
threat             478
insult            7877
identity_hate     1405




