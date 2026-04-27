# Product Feature Discussion Analysis using NLP

## Description
An NLP-based system that analyzes customer review text to extract and rank the most frequently discussed product features using the Bag-of-Words model and CountVectorizer.

This helps businesses understand which product attributes customers focus on most and prioritize improvements accordingly.

---

## Problem Statement
Customers frequently mention aspects such as battery life, camera quality, packaging, delivery, and price in product reviews. Manual analysis of large review datasets is inefficient and time-consuming.

This project automates the extraction and analysis of commonly discussed product features from review text.

---

## Objective
- Extract product-related terms from review text  
- Compute feature discussion frequency  
- Rank features by occurrence  
- Visualize top discussed product attributes  

---

## Methodology

### Step 1: Data Collection
Customer reviews are collected and stored in a structured format.

### Step 2: Text Vectorization
Review text is converted into numerical form using **CountVectorizer**, which performs:
- Lowercasing  
- Tokenization  
- Stopword Removal  
- Vocabulary Construction  
- Word Count Matrix Generation  

### Step 3: Feature Frequency Calculation
Word frequencies are aggregated across all reviews.

### Step 4: Ranking & Visualization
Features are ranked by frequency and visualized using a bar chart.

---

## Technical Implementation

### Algorithm Used: Bag-of-Words (BoW)
The Bag-of-Words model represents text as a frequency distribution of words while ignoring grammar and word order.

**Document Representation:**

D = [count(w₁), count(w₂), ..., count(wₙ)]

Where:
- **D** = Document Vector  
- **wₙ** = Vocabulary Terms  

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

## Sample Input

```text
Battery life is excellent but camera quality is average
The camera is amazing and battery lasts long
Price is too high for the features offered
Delivery was fast and packaging was good
```

---

## Sample Output

| Feature | Frequency |
|---------|----------|
| battery | 4 |
| camera | 3 |
| price | 2 |
| delivery | 2 |

---

## Applications
- Product Feedback Analysis  
- Customer Insight Generation  
- Market Research  
- Product Improvement Prioritization  

---

## Limitations
- Does not capture multi-word phrases unless n-grams are used  
- Frequency-based only; does not capture sentiment  
- Treats words independently without contextual understanding  

---

## Future Improvements
- Add N-Gram Phrase Detection  
- Perform Aspect-Based Sentiment Analysis  
- Use TF-IDF Weighting  
- Deploy as Web Dashboard  
