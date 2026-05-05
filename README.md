# Customer Segmentation: K-Means & Factor Analysis

A multivariate analysis project performing customer segmentation to optimize retail marketing strategies. This repository contains the technical execution and data preprocessing.

**[Read the full business case study and insights on Notion](https://www.notion.so/347f24b0444b80d382c0e5d57a613f1c?source=copy_link)**

---

## 📊 Overview
A groceries firm's database is used to conduct a customer personality analysis through market segmentation to optimize the significance of each customer to the business, such that the products can be modified according to the distinct needs and behaviours of the customers. This was achieved by using exploratory factor analysis (EFA) and cluster analysis, specifically Kmeans, to determine the market segments.


## 🎯 Key Findings
- Identified 4 factors through EFA that explain 64% of variance in purchasing behavior: Premium Shoppers, Household Buyers, Web Deal Seekers, and Teen Households.
- The combined factors of Premium Shoppers and Household Buyers represents the highest overall revenue opportunity. These are high-income customers who consistently purchase full-price items across catalog and in-store channels.
- Web Deal Seekers drive the bulk of online volume. This segment consists of moderate-income customers with financial constraints who are highly responsive to web-based promotions.


**Recommendation:** Feature full-priced premium products in catalogs and physical stores, while concentrating promotional campaigns and exclusive discounts on the website.
  
## 🔍 Methodology

**Data Source**: Anonymized customer data from [Kaggle](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis?select=marketing_campaign.csv) (50,000 records, 2020-2023)

**Approach**:
- Cleaned and preprocessed customer transaction data (handled 12% missing values)
- Scaled the data
- Identified the number of factors through Exploratory Factor Analysis (Python implementation adapted from this [tutorial](https://youtu.be/ttBs_wfw_6U?si=nnvSIggfTI80GDSN))
- Segmentation achieved through cluster analysis (Kmeans)

  
## 📁 Repository Structure
```text
customer-segmentation-efa-kmeans/
│
├── efa-kmeans.ipynb       # Main Jupyter Notebook with analysis
├── Customer data-1.csv    # Dataset used
├── .gitignore             # Hidden files and local environments to ignore
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
git clone https://github.com/jrph-data/customer-segmentation-efa-kmeans.git
cd customer-churn-prediction
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
