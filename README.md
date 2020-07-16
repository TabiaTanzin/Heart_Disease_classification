# Heart_Disease_classification

According to the National Heart, Lung and Blood Institute:

Heart disease is a catch-all phrase for a variety of conditions that affect the heart’s structure and function. Coronary heart disease is a type of heart disease that develops when the arteries of the heart cannot deliver enough oxygen-rich blood to the heart. It is the leading cause of death in the United States.

(Emphasis by me. Source: https://www.nhlbi.nih.gov/health-topics/espanol/enfermedad-coronaria)

Also, according to the World Health Organization, cardiovascular diseases are the leading cause of death globally (source: https://www.who.int/news-room/fact-sheets/detail/cardiovascular-diseases-(cvds)).

In this notebook we try to learn enough information of this topic to understand the Heart Disease UCI dataset and build simple models to predict whether a patient has a disease or not based on features like the heart rate during exercise or the cholesterol levels in the blood.


# Dataset & dataset problems

This dataset is hosted on Kaggle (Heart Disease UCI), and it was from UCI Machine Learning Repository. There are records of about 300 patients from Cleveland and the features are described in a following section.
Part of these differences is that there were a few null values in the original dataset that have taken some values here:

## A few more things to consider:
data
# 93, 159, 164, 165 and 252 have ca=4 which is incorrect. In the original Cleveland dataset they are NaNs (so they should be removed)
# 49 and 282 have thal = 0, also incorrect. They are also NaNs in the original dataset.
Because these are just a few instances, I decided to drop them.
There are also some differences regarding the features of the dataset which are corrected below.

