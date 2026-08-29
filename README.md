# Customer Segmentation: Factor Analysis & K-Means 

A multivariate analysis project performing customer segmentation to optimize retail marketing strategies. This repository contains the technical execution and data preprocessing.

**[Read the full business case study and insights on Notion](https://www.notion.so/347f24b0444b80d382c0e5d57a613f1c?source=copy_link)**

---

## 📊 Overview
A groceries firm's database is used to conduct a customer personality analysis through market segmentation to optimize the significance of each customer to the business to enable targeted marketing strategies. This was achieved by using exploratory factor analysis (EFA), cluster analysis and segment profiling.


## 🎯 Key Findings
- Reduced data dimensionality to 4 factors through EFA.
- Identified three market segments.
- The most profitable are consumers with the highest income that does in-store and catalog purchases and barely browses online offerings.
- This is followed by the old long-tenure customers with decent income who seek web deals and are responsive to online promotions.


**Recommendation:** Feature full-priced premium products in catalogs and physical stores, while concentrating promotional campaigns and exclusive discounts on the website.
  
## 🔍 Methodology

**Data Source**: Anonymized customer data from [Kaggle](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis?select=marketing_campaign.csv) (2,240 records)

**Approach**:
- Cleaned and preprocessed customer transaction data through converting time-related features into number of years, conversion into ordinal data and binary data through one-hot encoding.
- Scaled the numeric data.
- Identified the number of factors through Exploratory Factor Analysis (Python implementation adapted from this [tutorial](https://youtu.be/ttBs_wfw_6U?si=nnvSIggfTI80GDSN))
- Segmentation achieved through cluster analysis (Kmeans) through WCSS and Silhouette Score.
- Segments were profiled using the mean of unscaled data.

  
## 📁 Repository Structure
```text
customer-segmentation-efa-kmeans/
│
├── efa-kmeans.ipynb       # Main Jupyter Notebook with comprehsnive breakdown
├── Customer data-1.csv    # Dataset used
├── .gitignore             # Hidden files and local environments to ignore
├── requirements.txt       # Libraries used
└── README.md              # Technical documentation
```
## 🚀 Getting Started

### Prerequisites
* **Language:** Python 3.11.14
* **Environment:** Jupyter Notebook
* **Core Libraries:** `pandas`, `numpy`, `scikit-learn`, `factor_analyzer`, `matplotlib`, `seaborn`, `standard_scaler`, `datetime`, `pingouin`


### Installation

1. Clone this repository
```bash
!git clone https://github.com/jrph-data/customer-segmentation-efa-kmeans.git
%cd customer-segmentation-efa-kmeans
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Run the analysis
```bash
jupyter notebook efa-kmeans.ipynb
```
---
*This project was completed as part of my Data Science Masters program at De La Salle Univeristy*
