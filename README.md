# Customer Personality Segmentation

Unsupervised machine learning project that segments a retail company's 2,240-customer base into four distinct behavioral profiles using K-Means clustering — enabling targeted marketing, improved retention, and smarter resource allocation.

---

## Project Assets

| Asset | Description |
|---|---|
| [Analysis Notebook](Learner_Notebook_Low_Code_Version_Customer_Personality_Segmentation.ipynb) | End-to-end analysis: EDA, preprocessing, K-Means clustering, and cluster profiling |
| [Presentation Deck](SydneeSampsonBlackwell-CustomerSegmentation-Presentation.pptx%20(1)%20(1).pdf) | Business-facing slide deck with segment profiles and strategic recommendations |
| [Dataset](Customer_Personality_Segmentation.csv) | 2,240 customer records across 30 attributes (demographics, spending, purchase behavior) |

---

## Business Context

A leading retail company needed to move beyond generic marketing strategies. With an intensifying competitive landscape, personalized approaches became essential for sustaining growth and building long-term customer relationships.

**Goal:** Identify distinct customer segments to:
- Develop personalized marketing campaigns that increase conversion rates
- Build effective retention strategies for high-value customers
- Optimize resource allocation across inventory, pricing, and channels

---

## Dataset

**2,240 records · 30 features**

| Category | Features |
|---|---|
| Demographics | Year of birth, education, marital status, income, household composition |
| Spending (2 years) | Wine, fruits, meat, fish, sweets, gold products |
| Purchase Behavior | Web, catalog, and store purchases; deal usage |
| Campaign Response | Responses to 5 marketing campaigns |

---

## Methodology

```
Data Cleaning → EDA → Feature Scaling → K-Means → Cluster Profiling → Recommendations
```

1. **Data Cleaning** — Imputed 24 missing `Income` values; dropped irrelevant columns; confirmed zero duplicates
2. **EDA** — Univariate distributions (histograms + boxplots) and multivariate correlations (heatmap + pairplots)
3. **Preprocessing** — StandardScaler normalization before clustering
4. **Optimal K Selection** — Elbow method (WCSS) pointed to k=4; silhouette scores validated the choice
5. **Cluster Profiling** — Boxplots and barplots comparing income, spending, channel preference, and campaign response across segments

---

## Results: Four Customer Segments

### Cluster 1 — High-Value Enthusiasts
> High income · Heavy spenders on wine and meat · Catalog and store shoppers · Low discount sensitivity

**Strategy:** Premium loyalty program with exclusive access to high-margin products.

---

### Cluster 2 — Deal-Seeking Families
> Households with children/teens · Moderate income · High reliance on discounts

**Strategy:** Family-sized bundle promotions and discount coupons delivered via email.

---

### Cluster 0 — Opportunity Segment
> Lower income · High web traffic · Low conversion to actual purchases

**Strategy:** Welcome discounts and limited-time offers to convert browsers into buyers.

---

### Cluster 3 — Balanced Shoppers
> Mid-range income · Consistent cross-category spending · Frequent in-store shoppers

**Strategy:** Enhance in-store experience and promote Buy Online, Pick Up In Store (BOPIS).

---

## Key Findings

- **Income is the strongest spending predictor** — high positive correlation with wine and meat spend
- **Families spend differently** — households with children/teens show negative correlation with luxury category spending
- **Web visits ≠ spending** — lower-income customers browse most frequently but convert least
- **High-value customers are omnichannel** — Cluster 1 purchases actively across store, web, and catalog

---

## Tech Stack

`Python` · `pandas` · `NumPy` · `scikit-learn` · `Matplotlib` · `seaborn` · `yellowbrick`
