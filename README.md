# Product Feature Discussion Analysis using NLP

## Description
An NLP-based system that analyzes customer review text to extract and rank the most frequently discussed product features using the Bag-of-Words model and CountVectorizer.

This helps businesses understand which product attributes customers focus on most and prioritize improvements accordingly.

---

## Problem Statement
Customers frequently discuss product-related aspects such as battery life, camera quality, packaging, delivery, and price in reviews.

Manual analysis of large volumes of reviews is inefficient and time-consuming.

This project automates the extraction and analysis of commonly discussed product features from customer review text.

---

## Objective
- Extract product-related terms from review text  
- Compute frequency of discussed features  
- Rank features by frequency  
- Visualize top discussed product attributes  

---

## Algorithm / Methodology

### Step 1: Data Collection
Customer reviews are collected and stored in a structured format using a Pandas DataFrame.

---

### Step 2: Text Vectorization
The review text is transformed into numerical form using **CountVectorizer** from Scikit-learn.

CountVectorizer performs:
- Lowercasing  
- Tokenization  
- Stopword Removal  
- Vocabulary Construction  
- Word Count Matrix Generation  

---

### Step 3: Feature Frequency Calculation
Word frequencies are aggregated across all reviews to determine how often each feature is discussed.

---

### Step 4: Ranking
Features are sorted in descending order of frequency.

---

### Step 5: Visualization
A bar chart is generated to visualize the top discussed product features.

---

## Technical Implementation

### Algorithm Used
**Bag-of-Words (BoW)**

The Bag-of-Words model represents text as a frequency distribution of words, ignoring grammar and word order.

Each review is converted into a vector:

D = [count(w₁), count(w₂), count(w₃), ..., count(wₙ)]

Where:
- D = Document Vector  
- wₙ = Vocabulary Terms  

---

## Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Pandas | Data Handling |
| Scikit-learn | NLP Vectorization |
| Matplotlib | Visualization |

---

## Installation

```bash
pip install pandas matplotlib scikit-learn
```

---

## Usage

1. Clone the repository

```bash
git clone <your-repo-link>
```

2. Open Jupyter Notebook / Python Script

3. Run the program

---

## Sample Input

```text
Battery life is excellent but camera quality is average
The camera is amazing and battery lasts long
Price is too high for the features offered
Delivery was fast and packaging was good
```

---

## Sample Output

### Top Product Features

| Feature | Frequency |
|---------|----------|
| battery | 4 |
| camera | 3 |
| price | 2 |
| delivery | 2 |

---

## Visualization Output
Bar chart showing the top 10 discussed product features.

---

## Applications
- Product Feedback Analysis  
- Customer Insight Generation  
- Market Research  
- Product Improvement Prioritization  

---

## Limitations
- Does not capture multi-word phrases (e.g., "battery life") unless n-grams are used  
- Frequency-based only; does not capture sentiment  
- Treats words independently without context  

---

## Future Improvements
- Add N-Gram Phrase Detection  
- Perform Aspect-Based Sentiment Analysis  
- Use TF-IDF instead of raw frequency  
- Deploy as Web Dashboard  

---

## Conclusion
This project demonstrates how Natural Language Processing can be used to automatically extract actionable insights from customer review data by identifying frequently discussed product features.

It provides a scalable and efficient alternative to manual review analysis.

---
