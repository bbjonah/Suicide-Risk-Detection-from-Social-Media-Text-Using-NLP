# Suicide Risk Detection from Social Media Text Using NLP

![alt text](image.jpg)

An NLP-powered public health machine learning system for detecting suicide-risk signals from social media text. This project combines Natural Language Processing (NLP), psychological indicators, sentiment analysis, and machine learning to identify potential suicide risk patterns for **early-risk screening and population-level mental health surveillance**.

> **Disclaimer:**  
> This project is designed for **research, education, and public health analytics purposes only**. It is **NOT intended for clinical diagnosis, medical decision-making, or emergency mental health intervention**.

---

## Project Overview

Mental health challenges and suicidal ideation are increasingly reflected in online conversations and social media interactions. Detecting distress signals early can support **preventive mental health strategies** and **digital epidemiology research**.

This project leverages:

- **Natural Language Processing (NLP)**
- **Machine Learning Classification**
- **Sentiment Analysis**
- **Behavioral Risk Indicators**
- **Public Health Analytics**
- **Geospatial Mental Health Insights**

to classify social media posts into suicide-risk categories.

The system analyzes social media text patterns and combines them with simulated psychological indicators to classify posts as:

- **Low Risk**
- **Moderate Risk**
- **High Risk**

---

## Objectives

The primary objectives of this project are to:

- Detect suicide-risk signals from social media text
- Identify linguistic patterns linked to emotional distress
- Build predictive NLP models for suicide-risk classification
- Analyze sentiment and behavioral indicators
- Visualize mental health risk trends across demographics and locations
- Demonstrate ethical AI applications in public health surveillance

---

## Key Features

### NLP Text Processing
- Text cleaning
- Tokenization
- Stopword removal
- URL and punctuation removal
- Social media text normalization

### Machine Learning Models
- Logistic Regression
- Random Forest Classifier

### Feature Engineering
The model combines text with psychological indicators:

| Feature | Description |
|----------|-------------|
| Text | Social media content |
| Sentiment Score | Emotional polarity |
| Depression Score | Simulated psychological distress |
| Anxiety Score | Anxiety-related indicator |
| Sleep Issues | Sleep disruption indicator |
| Social Isolation Score | Isolation signal |
| Self-Harm Keywords | Presence of crisis-related terms |

### Advanced Analytics
- Suicide-risk classification
- Sentiment trend analysis
- Psychological feature importance
- Word cloud generation
- Confusion matrix evaluation
- Platform-wise risk analysis
- Risk distribution visualization

---

## Dataset Description

This project uses a **large realistic synthetic dataset** containing **25,000+ simulated social media posts**.

### Dataset Features

| Column | Description |
|--------|-------------|
| post_id | Unique identifier |
| text | Social media post text |
| timestamp | Date and time |
| age_group | User age category |
| gender | Simulated demographic |
| state | Nigerian state |
| platform | Social media source |
| sentiment_score | Emotional sentiment |
| depression_score | Psychological distress |
| anxiety_score | Anxiety indicator |
| sleep_issue_score | Sleep disruption |
| social_isolation_score | Isolation metric |
| self_harm_keywords | Crisis keyword indicator |
| crisis_keyword_flag | High-risk keyword presence |
| risk_level | Low / Moderate / High |
| label | Binary target variable |

### Risk Labels

| Label | Meaning |
|--------|---------|
| 0 | Low Risk |
| 1 | Suicide Risk |

---

## Project Structure

```text
Suicide-Risk-Detection-from-Social-Media-Text-Using-NLP/
│
├── data/
│   └── suicide_risk_social_media_nlp_dataset.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── visuals/
│   ├── dashboard.png
│   ├── wordcloud.png
│   ├── confusion_matrix.png
│   └── charts/
│
├── models/
│   └── suicide_risk_model.pkl
│
├── suicide_risk_detection.py
├── requirements.txt
├── README.md
└── LICENSE
```

---

## Methodology

### 1. Data Collection
A realistic synthetic dataset simulates:

- General social media posts
- Emotional distress
- Anxiety symptoms
- Depression-related language
- High-risk suicidal ideation indicators

---

### 2. NLP Pipeline

The text preprocessing workflow includes:

```python
Lowercasing
↓
Remove URLs
↓
Remove punctuation
↓
Remove numbers
↓
Text normalization
↓
TF-IDF Vectorization
```

The cleaned text is transformed into numerical representations using:

### TF-IDF Vectorization
- Unigrams
- Bigrams
- High-dimensional sparse features

---

### 3. Machine Learning Pipeline

Two supervised learning models are implemented:

#### Logistic Regression
A lightweight baseline NLP classifier.

#### Random Forest
A robust ensemble learning model for improved prediction.

---

### 4. Model Evaluation

Performance is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

> **Why Recall Matters Most:**  
> In suicide-risk detection, false negatives are costly because failing to identify a high-risk post could have severe consequences. Therefore, recall is prioritized.

---

## Exploratory Data Analysis (EDA)

The project generates insightful analytics such as:

### Risk Level Distribution
Understanding class balance across suicide-risk categories.

### Sentiment vs Risk Analysis
Relationship between emotional polarity and risk.

### Platform-wise Suicide Risk Rate
Comparing risk prevalence across platforms.

### Psychological Feature Importance
Identifying major indicators influencing prediction.

### Word Cloud Visualization
Most common terms in high-risk posts.

### Time-Based Risk Trends
Mental health signal fluctuations over time.

### Geospatial Mental Health Analytics
State-level risk distribution across Nigeria.

---

## Geospatial Analytics

This project supports **GIS-style mental health surveillance** using Nigerian state-level data.

Potential outputs include:

- Suicide-risk heatmaps
- High-risk state clusters
- Regional psychological distress patterns
- Public health intervention mapping

Example:

```text
High Risk Concentration
Lagos ████████
Kaduna ██████
Abuja █████
Rivers █████
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Suicide-Risk-Detection-from-Social-Media-Text-Using-NLP.git
```

Move into the project folder:

```bash
cd Suicide-Risk-Detection-from-Social-Media-Text-Using-NLP
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Required Dependencies

```txt
pandas
numpy
matplotlib
scikit-learn
wordcloud
joblib
```

Install manually:

```bash
pip install pandas numpy matplotlib scikit-learn wordcloud joblib
```

---

## Running the Project

Run the Python script:

```bash
python suicide_risk_detection.py
```

Outputs generated:

- Trained NLP model
- Evaluation metrics
- Confusion matrix
- Risk visualizations
- Word cloud
- Model artifact (`.pkl`)

---

## Example Prediction

Input:

```text
"I feel hopeless and alone. Nobody understands me anymore."
```

Output:

```text
Suicide Risk Detected
```

---

## Sample Visualizations

Recommended portfolio visualizations:

- Risk level distribution chart
- Sentiment vs suicide-risk graph
- Word cloud of distress keywords
- Psychological feature importance
- Nigeria geospatial heatmap
- Confusion matrix
- Monthly suicide-risk trends
- Platform comparison dashboard

---

## Ethical Considerations

Mental health prediction systems require responsible deployment.

### Important Ethical Notes

- This model should **never replace mental health professionals**
- Predictions may contain uncertainty
- False positives and false negatives are possible
- Privacy and consent are critical in real-world systems
- Human oversight is essential

This project is intended strictly for:

✅ Research  
✅ Public health analytics  
✅ Education  
✅ Portfolio demonstration

---

## Future Improvements

Potential upgrades include:

- Deep Learning (LSTM, GRU)
- Transformer Models (BERT, DistilBERT)
- Real-time dashboard deployment
- Explainable AI (SHAP/LIME)
- Multi-class suicide severity prediction
- Real social media streaming simulation
- Temporal forecasting models

---

## Results

The model successfully demonstrates:

- NLP-based suicide-risk detection
- Emotional distress signal identification
- Psychological feature integration
- Public health mental health analytics
- Explainable predictive modeling

---

## Author

**Jonah Buka**  
Data Scientist | Public Health Analytics | Machine Learning | NLP

---

## License

This project is licensed under the **MIT License**.

---

## Support

If you found this project useful:

⭐ Star the repository  
🍴 Fork the project  
📢 Share with the data science community
