# HeartDetect

![Python](http://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=ffffff)

An Analytical Model For Early Intervention Of Cardiovascular Disease, implemented in `2 stages`

### Jupyter notebooks
- data-cleaning-preprocessing.ipynb
- exploratory-data-analysis_1.ipynb
- exploratory-data-analysis_2.ipynb
- stage1-modelling.ipynb
- stage2-modelling.ipynb

<br/>

# Getting Started

### 1. Clone a copy of this repository
Open your terminal and run
```
git clone https://github.com/xJQx/bc2406-project.git
```

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

### 3. Understanding the various csv files

**Dataset created from the `data-cleaning-preprocessing.ipynb` notebook:**

    .
    ├── heart_pki_2020_original.csv       # original dataset
    |   ├── heart_pki_2020_cleaned.csv        # for EDA and visualization
    |   └── heart_pki_2020_correlation.csv    # for EDA correlation (some OneHotEncoding done)
    |   └── heart_pki_2020_encoded.csv        # for analytical models (OneHotEncoding done)
    |
    ├── o2Saturation_original.csv         # original dataset
    ├── heart_attack_original.csv         # original dataset
    │   ├── heart_attack_cleaned.csv          # for EDA and analytical model (default integer encoding)
    │   └── heart_attack_cleaned_text.csv     # for EDA and visualization (meaningful values)
    └──|



