# Product Feature Discussion Analysis using NLP

## Description
This project analyzes Amazon customer review text to identify the product features most frequently discussed by customers. Using Natural Language Processing techniques, review data is processed and transformed into numerical form using the Bag-of-Words model with CountVectorizer.

The analysis helps determine which product attributes customers focus on most, enabling businesses to better understand customer priorities and identify areas for product improvement.

---

## Problem Statement
Customers often discuss specific product features such as battery life, camera quality, packaging, delivery time, or price in product reviews. Understanding which features are mentioned most frequently can help companies prioritize improvements and make data-driven product decisions.

---

## Objective
- Extract frequently discussed product-related terms from customer reviews  
- Analyze which product features matter most to customers  
- Visualize the frequency distribution of discussed features  

---

## Methodology
1. Loaded and inspected the Amazon reviews dataset  
2. Cleaned the dataset by removing irrelevant columns, duplicates, and missing values  
3. Extracted review text for NLP analysis  
4. Applied CountVectorizer using the Bag-of-Words model  
5. Used n-grams and custom stopword filtering to improve feature extraction quality  
6. Computed feature frequencies across all reviews  
7. Visualized extracted features using multiple charts  

---

## Technologies Used
- Python  
- Pandas  
- Scikit-learn  
- Matplotlib  
- Seaborn  
- WordCloud  

---

## Output
The project generates:
- Ranked table of most discussed product features  
- Bar chart of top discussed features  
- Pie chart of feature distribution  
- Word cloud of extracted product attributes  

---

## Applications
- Customer Feedback Analysis  
- Product Improvement Prioritization  
- Market Research  
- Consumer Preference Analysis  

---

## Future Improvements
- Apply Part-of-Speech tagging for more accurate noun/feature extraction  
- Perform Aspect-Based Sentiment Analysis on extracted features  
- Replace Bag-of-Words with TF-IDF or Transformer-based embeddings  
