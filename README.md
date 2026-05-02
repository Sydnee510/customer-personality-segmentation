<div align="center">

# 🛍️ Customer Personality Segmentation

### Unsupervised Machine Learning · Retail Analytics · K-Means Clustering

*Segmenting a 2,240-customer retail base into four behavioral profiles to enable targeted marketing, smarter retention, and optimized resource allocation.*

<br>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)

<br>

</div>

---

## 📁 Project Assets

| Asset | Description |
|:---|:---|
| 📓 [Analysis Notebook](Learner_Notebook_Low_Code_Version_Customer_Personality_Segmentation.ipynb) | End-to-end analysis: EDA, preprocessing, K-Means clustering, and cluster profiling |
| 📊 [Presentation Deck](SydneeSampsonBlackwell-CustomerSegmentation-Presentation.pptx%20(1)%20(1).pdf) | Business-facing slide deck with segment profiles and strategic recommendations |
| 🗂️ [Dataset](Customer_Personality_Segmentation.csv) | 2,240 customer records across 30 attributes |

---

## 🧠 Business Context

A leading retail company needed to move beyond generic marketing strategies. With an intensifying competitive landscape, personalized approaches became essential for sustaining growth and building long-term customer relationships.

**Goal:** Identify distinct customer segments to:
- 📈 Develop personalized marketing campaigns that increase conversion rates
- 🤝 Build effective retention strategies for high-value customers
- 📦 Optimize resource allocation across inventory, pricing, and channels

---

## 📊 Dataset

<div align="center">

**2,240 records · 30 features**

</div>

| Category | Features |
|:---|:---|
| 👤 Demographics | Year of birth, education, marital status, income, household composition |
| 💳 Spending (2 years) | Wine, fruits, meat, fish, sweets, gold products |
| 🛒 Purchase Behavior | Web, catalog, and store purchases; deal usage |
| 📣 Campaign Response | Responses to 5 marketing campaigns |

---

## ⚙️ Methodology

<div align="center">

```
Data Cleaning  →  EDA  →  Feature Scaling  →  K-Means  →  Cluster Profiling  →  Recommendations
```

</div>

| Step | Action |
|:---:|:---|
| 1 | **Data Cleaning** — Imputed 24 missing `Income` values; dropped irrelevant columns; confirmed zero duplicates |
| 2 | **EDA** — Univariate distributions (histograms + boxplots) and multivariate correlations (heatmap + pairplots) |
| 3 | **Preprocessing** — StandardScaler normalization before clustering |
| 4 | **Optimal K Selection** — Elbow method (WCSS) pointed to k=4; silhouette scores validated the choice |
| 5 | **Cluster Profiling** — Boxplots and barplots comparing income, spending, channel preference, and campaign response |

---

## 🎯 Results: Four Customer Segments

### ![#gold](https://img.shields.io/badge/Cluster_1-High--Value_Enthusiasts-FFB300?style=flat-square)
> 💰 High income · Heavy spenders on wine and meat · Catalog and store shoppers · Low discount sensitivity

**Strategy:** Premium loyalty program with exclusive access to high-margin products.

<br>

### ![#blue](https://img.shields.io/badge/Cluster_2-Deal--Seeking_Families-1565C0?style=flat-square)
> 👨‍👩‍👧‍👦 Households with children/teens · Moderate income · High reliance on discounts

**Strategy:** Family-sized bundle promotions and discount coupons delivered via email.

<br>

### ![#green](https://img.shields.io/badge/Cluster_0-Opportunity_Segment-2E7D32?style=flat-square)
> 🌐 Lower income · High web traffic · Low conversion to actual purchases

**Strategy:** Welcome discounts and limited-time offers to convert browsers into buyers.

<br>

### ![#purple](https://img.shields.io/badge/Cluster_3-Balanced_Shoppers-6A1B9A?style=flat-square)
> ⚖️ Mid-range income · Consistent cross-category spending · Frequent in-store shoppers

**Strategy:** Enhance in-store experience and promote Buy Online, Pick Up In Store (BOPIS).

---

## 💡 Key Findings

| Finding | Insight |
|:---|:---|
| 📊 Income drives spending | Strong positive correlation with wine and meat categories |
| 👨‍👩‍👧 Families spend differently | Children/teens in household negatively correlates with luxury spend |
| 🖥️ Web visits ≠ spending | Lower-income customers browse most but convert least |
| 🔄 High-value = omnichannel | Top spenders are active across store, web, and catalog |

---

<div align="center">

*MIT Applied Data Science Program · Making Sense of Unstructured Data*

</div>
