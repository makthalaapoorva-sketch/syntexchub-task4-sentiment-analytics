# syntexchub-task4-sentiment-analytics
# 📊 Amazon Product Reviews Sentiment Analysis Dashboard

An interactive Power BI data analytics solution exploring e-commerce feedback trends, customer sentiment distribution, and brand-level performance ratings.

## 🛠️ Project Overview
This project processes and visualizes a sample dataset of Amazon product reviews (`amazon_com-product_reviews__20200101_20200331_sample`) to extract actionable consumer behavior insights.

### 📌 Key Dashboard Metrics & Features
- **Total Reviews Analyzed:** 50
- **Sentiment Breakdown:** Categorized reviews into Positive (78%), Negative (16%), and Neutral (6%) proportions using custom calculated columns and DAX conditional rules.
- **Rating Distribution:** Evaluated customer satisfaction levels across 1 to 5 star ratings.
- **Brand & Category Performance:** Mapped high-performing brands (*Dove, Schmidt's, SheaMoisture, Talenti*) against positive/negative percentages.

## 📈 DAX Measures Implemented
* `Total Reviews = COUNTROWS('amazon_com-product_reviews__20200101_20200331_sample')`
* `Positive Count = CALCULATE(COUNTROWS(...), [Sentiment] = "Positive")`
* `Negative Count = CALCULATE(COUNTROWS(...), [Sentiment] = "Negative")`
* `Positive Percentage = DIVIDE([Positive Count], [Total Reviews], 0)`
* `Negative Percentage = DIVIDE([Negative Count], [Total Reviews], 0)`

## 🚀 How to View
1. Download the `.pbix` file from this repository.
2. Open it using **Power BI Desktop**.
