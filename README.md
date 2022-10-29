# HeartDetect 💘

![Python](http://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=ffffff)

An Analytical Model For Early Intervention Of Heart Disease, implemented in `2 stages`

### Jupyter notebooks
- [data-cleaning-preprocessing.ipynb](https://github.com/xJQx/bc2406-project/blob/main/data-cleaning-preprocessing.ipynb)
- [exploratory-data-analysis_1.ipynb](https://github.com/xJQx/bc2406-project/blob/main/exploratory-data-analysis_1.ipynb)
- [exploratory-data-analysis_2.ipynb](https://github.com/xJQx/bc2406-project/blob/main/exploratory-data-analysis_2.ipynb)
- [stage1-modelling.ipynb](https://github.com/xJQx/bc2406-project/blob/main/stage1-modelling.ipynb)
- [stage2-modelling.ipynb](https://github.com/xJQx/bc2406-project/blob/main/stage2-modelling.ipynb)


<br/>

# Executive Summary

This report aims to deploy data analytics to solve the business problem for National Heart Centre Singapore (NHCS). Given the increasing incidence of reported cases of cardiovascular disease (CVD) in Singapore, NHCS handles more than **120,000** outpatient consultations each year. The sudden onset of heart disease is severe and expensive to treat. Therefore, NHCS can shift the **focus to early prevention rather than treating post-diagnosis.**
<br/>

To increase the involvement of individuals and primary care sectors in the prevention of heart disease, our team proposes a **2-step solution – HeartDetect.** 
- The first stage is to raise individuals' awareness and manage their heart health regularly. 
- The second stage is to enable the prediction of heart disease risk in the primary care sector to provide timely prevention.

<br/>

# Getting Started

### 1. Clone a copy of this repository
Open your terminal and run
```
git clone https://github.com/xJQx/bc2406-project.git
```

<br/>

### 2. Understanding the jupyter nodebook flow
**Data Cleaning and Pre-processing** <br>
a) [data-cleaning-preprocessing.ipynb](https://github.com/xJQx/bc2406-project/blob/main/data-cleaning-preprocessing.ipynb) <br>


**Stage 1:** <br>
b) [exploratory-data-analysis_1.ipynb](https://github.com/xJQx/bc2406-project/blob/main/exploratory-data-analysis_1.ipynb) <br>
c) [stage1-modelling.ipynb](https://github.com/xJQx/bc2406-project/blob/main/stage1-modelling.ipynb) <br>

**Stage 2:**  <br>
d) [exploratory-data-analysis_2.ipynb](https://github.com/xJQx/bc2406-project/blob/main/exploratory-data-analysis_2.ipynb) <br>
e) [stage2-modelling.ipynb](https://github.com/xJQx/bc2406-project/blob/main/stage2-modelling.ipynb) <br>

<br/>

### 3. Understanding the various csv files (datasets)

**Dataset created from the `data-cleaning-preprocessing.ipynb` notebook:**

    .
    ├── heart_pki_2020_original.csv       # original dataset
    |   ├── heart_pki_2020_cleaned.csv        # for EDA and visualization
    |   └── heart_pki_2020_correlation.csv    # for EDA correlation (IntegerEncoding done)
    |   └── heart_pki_2020_encoded.csv        # for analytical models (OneHotEncoding done)
    |
    ├── o2Saturation_original.csv         # original dataset
    ├── heart_attack_original.csv         # original dataset
    │   ├── heart_attack_cleaned.csv          # for EDA and analytical model (default integer encoding)
    │   └── heart_attack_cleaned_text.csv     # for EDA and visualization (meaningful values)
    └──|

<br/>

### 4. Understanding the models directory

The models directory contain all the trained models from stages 1 and 2. They can be imported and used for a dataset that fits their data dimensions. <br>
**An example of importing and using an analytical model is as shown:**

```
# Library
import joblib

# Load the model from disk
loaded_random_forest_m3 = joblib.load('models/stage2_random_forest_m3.sav')

# Using the analytical model
result = cross_val_score(loaded_random_forest_m3, X_test, y_test, cv=5, scoring = "roc_auc").mean()
print(result)
```


<br/>

# Contributors

<a href='https://github.com/xJQx' title='xJQx'> <img src='https://avatars.githubusercontent.com/xJQx' height='75' width='75'/></a>
<a href='https://github.com/zonpig' title='zonpig'> <img src='https://avatars.githubusercontent.com/zonpig' height='75' width='75'/></a>
<a href='https://github.com/leileijng' title='leileijng'> <img src='https://avatars.githubusercontent.com/leileijng' height='75' width='75'/></a>
<a href='https://github.com/geraldd-d' title='geraldd-d'> <img src='https://avatars.githubusercontent.com/geraldd-d' height='75' width='75'/></a>
<a href='https://github.com/zhihaohong52' title='zhihaohong52'> <img src='https://avatars.githubusercontent.com/zhihaohong52' height='75' width='75'/></a>
<a href='https://github.com/zainab1210' title='zainab1210'> <img src='https://avatars.githubusercontent.com/zainab1210' height='75' width='75'/></a>

