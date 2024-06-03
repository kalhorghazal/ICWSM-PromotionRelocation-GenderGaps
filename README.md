# ICWSM-PromotionRelocation-GenderGaps

This repository contains the dataset and analysis code for the paper:

**Title:** "Gender Gaps in Online Social Connectivity, Promotion and Relocation Reports on LinkedIn"

**Authors:** Ghazal Kalhor, Hannah Gardner, Ingmar Weber, and Ridhi Kashyap

**DOI:** https://doi.org/10.1609/icwsm.v18i1.31353

If you use our dataset or analysis code in your work, please cite our paper:

Kalhor, G., Gardner, H., Weber, I., & Kashyap, R. (2024). Gender Gaps in Online Social Connectivity, Promotion and Relocation Reports on LinkedIn. Proceedings of the *International AAAI Conference on Web and Social Media, 18*(1), 800-812. https://doi.org/10.1609/icwsm.v18i1.31353

## Dataset
We collected the following features, along with the audience estimate, for each combination of attributes:

* Country
* Gender
* Job Seniority
* Age Range
* Recent Status
* Social Connectivity
* Count


```python
import pandas as pd

fullData = pd.read_csv('fullData.csv')
fullData.head(3)
```

|Country|Gender|Job Seniority|Age Range|Recent Status|Social Connectivity|Count|
|----|----|----|----|----|----|----|
|US|Female|Director|55+|Any|Connected to big companies|8200|
|US|Female|Director|55+|Any|Any|19000|
|US|Female|Director|35 to 54|Relocated|Any|390|

```python
promotionData = pd.read_csv('promotionData.csv')
promotionData.head(3)
```

|Country|Gender|Job Seniority|Age Range|Recent Status|Social Connectivity|Count|
|----|----|----|----|----|----|----|
|US|Female|Director|55+|Not promoted|Connected to big companies|8200|
|US|Female|Director|55+|Not promoted|Not connected|10800|
|US|Female|Director|35 to 54|Recently promoted|Connected to big companies|2600|

```python
relocationData = pd.read_csv('relocationData.csv')
relocationData.head(3)
```

|Country|Gender|Job Seniority|Age Range|Recent Status|Social Connectivity|Count|
|----|----|----|----|----|----|----|
|US|Female|Director|55+|Not relocated|Connected to big companies|8200|
|US|Female|Director|55+|Not relocated|Not connected|10800|
|US|Female|Director|35 to 54|Recently relocated|Not connected|390|
