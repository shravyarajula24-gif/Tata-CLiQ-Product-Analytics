# Tata-CLiQ-Product-Analytics

## 📌 Overview
This project analyzes 500+ Kurtis scraped from Tata CLiQ to decode brand dominance, pricing strategy, discount psychology and customer ratings in Indian ethnic wear market.

We move from raw HTML → Clean Data → EDA → Statistical Testing → Business Insights

## 🎯 Objective
- Identify top brands in kurtis category
- Analyze price & discount distribution
- Check if brand influences price/discount
- Understand relation between price, discount and ratings

## 📊 Dataset
- **Source:** Tata CLiQ Website (https://www.tatacliq.com)
- **Records:** 500+ Kurtis
- **Columns:** Product Name, Brand, Price, Discount %, Rating, MRP, Selling Price
- **Tool Used for Scraping:** Selenium + BeautifulSoup

## 🛠️ Tech Stack
- **Language:** Python
- **Scraping:** Selenium, BeautifulSoup
- **Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Statistics:** SciPy (Z-Test, Chi-Square, ANOVA)
- **Environment:** Jupyter Notebook

## 🔄 Workflow
1.  **Web Scraping** - Scraped product cards using Selenium
2.  **Data Cleaning** - Handled missing values, removed duplicates, converted price to numeric
3.  **EDA** - Univariate & Bivariate analysis on Brand, Price, Discount, Rating
4.  **Hypothesis Testing**
    - Z-Test: Is avg price different from 1500?
    - Chi-Square: Is Brand associated with High Discount?
    - ANOVA: Does price vary by Brand?
5.  **Business Insights**

## 💡 Key Insights
- **Rangmanch, Libas, Biba** dominate >40% of listings
- **Average Price:** Rs. 1215 | Most common discount: 50-60%
- **Premium Brand:** AARKE (Avg Rs. 4500) vs **Budget:** Rangmanch (Avg Rs. 800)
- **Discount Strategy:** Libas gives 17 products with >60% discount, Fabindia gives 0 - Premium image
- **Correlation:** Price vs Rating = -0.15 (Weak negative) - High price ≠ High rating

## 📈 Statistical Results
- **Z-Test:** p-value < 0.05 - Average price is significantly different from 1500
- **Chi-Square Test:** Chi2 = 46.10, p = 2.42e-09 - Brand and High Discount are dependent
- **ANOVA:** F = 22.17, p = 4.83e-16 - Brand significantly influences Price

## 📁 Folder Structure
TataCLiQ-Kurtis-Analysis/
├── TataCLiQ_Scraping.ipynb
├── TataCLiQ_Cleaned_Data.csv
├── EDA_Visualizations/
├── README.md
└── requirements.txt

## ▶️ How to Run
```bash
pip install selenium beautifulsoup4 pandas numpy matplotlib seaborn scipy
jupyter notebook TataCLiQ_Scraping.ipynb
## 🚀 Future Scope
- Sentiment Analysis on Customer Reviews
- Price Prediction Model using ML
- Interactive Dashboard in Power BI / Tableau
- Daily automated scraping & trend tracking

## 👩‍💻 Author
*Shravya* | Aspiring Data Analyst | Innomatics Research Labs

## 🙏 Acknowledgements
Thanks to Tasleema Noor & Mamidi Swathi for mentorship

Want me to make a short version also for GitHub description box?
