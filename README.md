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

```
+----------------------+---------+
|       Field 1        | Field 2 |
+----------------------+---------+
|    Total Comments    |  159571 |
| Total clean comments |  143346 |
|     Total labels     |  35098  |
+----------------------+---------+
```

Comments per Label
```
toxic            15294
severe_toxic      1595
obscene           8449
threat             478
insult            7877
identity_hate     1405
```

Pearson Correlation Coefficient also referred to Pearson's R or the bivariate correlation is a statistic that measures the linear correlation between variables X and Y

![Pearson Correlation Coefficient](https://user-images.githubusercontent.com/14051949/153311536-df688b6f-c009-4039-8f19-8b71e0d6fff8.png)

Venn Diagram

Though the correlation between toxic and severe_toxic is just 0.31, but below Venn diagram shows that all severe_toxic are toxic comments. Indicating there is a non linear relationship between them that is not captured in the Pearson coefficient.

![toxic-severe_toxic](https://user-images.githubusercontent.com/14051949/153311858-5ba4de4b-4580-4550-a4c4-53f1ffac0caf.png)


Top 50 Words in Unprocessed Dataset
![3 Top 50 words - unprocessed data](https://user-images.githubusercontent.com/14051949/153312349-c0fe10a4-713f-45e0-bc06-a4c8c9c677cd.png)

The above barchart doesn't show any of the toxic words, and is basically filled with stop words.

Another great way to visualize is via WordClouds

Visualizing non toxic comments, for toxic comments word cloud refer to the ipynb in the repo.
![clean](https://user-images.githubusercontent.com/14051949/153312554-095c7e1f-46ae-4b91-8ae9-ad42b1f09f56.png)


