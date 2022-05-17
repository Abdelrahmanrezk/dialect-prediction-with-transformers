Arabic dialects, multi-class-Classification, Tweets.

# Dataset Card for Arabic_Dialect_Identification

## Table of Contents
- [Dataset Description](#dataset-description)
  - [Dataset Summary](#dataset-summary)
  - [Supported Tasks](#supported-tasks-and-leaderboards)
  - [Languages](#languages)
- [Dataset Structure](#dataset-structure)
  - [Data Instances](#data-instances)
  - [Data Fields](#data-instances)
  - [Data Splits](#data-instances)
- [Dataset Creation](#dataset-creation)
  - [Curation Rationale](#curation-rationale)
  - [Source Data](#source-data)
  - [Annotations](#annotations)
  - [Personal and Sensitive Information](#personal-and-sensitive-information)
- [Considerations for Using the Data](#considerations-for-using-the-data)
  - [Social Impact of Dataset](#social-impact-of-dataset)
  - [Discussion of Biases](#discussion-of-biases)
  - [Other Known Limitations](#other-known-limitations)
- [Additional Information](#additional-information)
  - [Dataset Curators](#dataset-curators)
  - [Licensing Information](#licensing-information)
  - [Citation Information](#citation-information)

## Dataset Description

- **Homepage:** [Needs More Information]
- **Repository:** https://github.com/Abdelrahmanrezk/dialect-prediction-with-transformers
- **Paper:** https://arxiv.org/pdf/2005.06557.pdf
- **Leaderboard:** Abdelrahmanrezk@acm.org
Aiman.Mahgoub@ul.ie
Conor.Ryan@ul.ie
- **Point of Contact:** Abdelrahmanrezk@acm.org
Aiman.Mahgoub@ul.ie
Conor.Ryan@ul.ie

### Dataset Summary

We present QADI, an automatically collected dataset of tweets belonging to a wide range of
country-level Arabic dialects covering 18 different countries in the Middle East and North
Africa region. Our method for building this dataset relies on applying multiple filters to identify
users who belong to different countries based on their account descriptions and to eliminate
tweets that are either written in Modern Standard Arabic or contain inappropriate language. The
resultant dataset contains 540k tweets from 2,525 users who are evenly distributed across 18 Arab countries. 

### Supported Tasks and Leaderboards

- Multi-class-Classification: Using extrinsic evaluation, we are able to build effective country-level dialect identification on tweets with a macro-averaged F1-score of 51.5% across 18 classes. 
[Arabic-Dialect-Identification](https://github.com/Abdelrahmanrezk/Arabic-Dialect-Identification), rather than what used in the paper Using intrinsic evaluation, they show that the labels of a set of randomly selected tweets are 91.5% accurate. For extrinsic evaluation, they are able to build effective country-level dialect identification on tweets with a macro-averaged F1-score of 60.6% across 18 classes [ Paper](https://arxiv.org/pdf/2005.06557.pdf). And we aimed by next work to fine tune models with that data to see how the result will be.

### Languages

Arabic

## Dataset Structure

### Data Instances
'{"id": [1159906099585327104, 950123809608171648, 1091295506960142336], "label": [10, 14, 2], "text": ["ايه الخيبة و الهرتلة قدام الجون دول؟؟ \U0001f92a😲\\nالعيال دي تتعلق في الفلكة يا معلم كلوب", "@FIA_WIS تذكرت ما اسمي عائشة انا اسمي خولة", "@showqiy @3nood_mh لا والله نروح نشجع قطر و نفرح معهم وش رايك بعد"]}'


### Data Fields


'"{\'id\': Value(dtype=\'int64\', id=None), \'label\': ClassLabel(num_classes=18, names=[\'OM\', \'SD\', \'SA\', \'KW\', \'QA\', \'LB\', \'JO\', \'SY\', \'IQ\', \'MA\', \'EG\', \'PL\', \'YE\', \'BH\', \'DZ\', \'AE\', \'TN\', \'LY\'], id=None), \'text\': Value(dtype=\'string\', id=None)}"'

### Data Splits

This dataset is split into a train, validation and test split. The split sizes are as follow:

|Split name	|  Number of samples |
|------------- | ---------- |
|train | 440052 |
|validation | 9164 |
|test | 8981 |

## Dataset Creation

### Curation Rationale

[Needs More Information]

### Source Data

#### Initial Data Collection and Normalization

[Needs More Information]

#### Who are the source language producers?

[Needs More Information]

### Annotations

#### Annotation process

[Needs More Information]

#### Who are the annotators?

[Needs More Information]

### Personal and Sensitive Information

[Needs More Information]

## Considerations for Using the Data

### Social Impact of Dataset

[Needs More Information]

### Discussion of Biases

[Needs More Information]

### Other Known Limitations

[Needs More Information]

## Additional Information

### Dataset Curators

{aabdelali,hmubarak,ysamih,sahassan2,kdarwish}@hbku.edu.qa

### Licensing Information

[Needs More Information]

### Citation Information

@unknown{unknown,
author = {Abdelali, Ahmed and Mubarak, Hamdy and Samih, Younes and Hassan, Sabit and Darwish, Kareem},
year = {2020},
month = {05},
pages = {},
title = {Arabic Dialect Identification in the Wild}
}
