# BC2406 Project: Analytical Model For Early Intervention Of Cardiovascular Disease

![Python](http://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=ffffff)

### Jupyter notebooks

- data-cleaning-preprocessing.ipynb

<br/>

### 1. Data cleaning and pre-processing

**Dataset created from the `data-cleaning-preprocessing.ipynb` notebook:**

    .
    ├── heart_pki_2020_original.csv       # original dataset
    |   ├── heart_pki_2020_cleaned.csv        # for EDA and visualization
    |   └── heart_pki_2020_encoded.csv        # for analytical models (OneHotEncoding done)
    |   └── heart_pki_2020_correlation.csv    # for correlation (some OneHotEncoding done)
    |
    ├── o2Saturation_original.csv         # original dataset
    ├── heart_attack_original.csv         # original dataset
    │   ├── heart_attack_cleaned.csv          # for analytical model (default integer encoding)
    │   └── heart_attack_cleaned_text.csv     # for EDA and visualization (meaningful values)
    └──|
