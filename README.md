# 🌍 Climate Change Modeling & Sentiment Analysis

This project presents a complete machine learning pipeline to analyze **climate-related sentiments** using real-world data. By combining natural language processing, exploratory data analysis, and supervised learning, it captures emotional trends, predicts sentiment polarity, and provides visual interpretations to support environmental insights and awareness.

---

## 🎯 Objective

The objective of this project is to develop a machine learning-based model to analyze and predict the impact of various factors contributing to climate change, specifically public sentiment expressed through text. Using historical and real-time environmental discussion data, the model:

- Classifies text into Positive, Neutral, or Negative sentiments
- Uses likes and comment engagement as indicators of sentiment
- Supports policy makers and researchers with interpretable sentiment trends
- Visualizes climate communication to raise awareness

---

## 🔍 Project Highlights

### 📥 Data Collection & Preprocessing
- Dataset includes: `date`, `likesCount`, `commentsCount`, `text`, `profileName`
- Text cleaning includes removal of punctuation, lowercasing, stopword removal, and lemmatization
- Null value treatment for comments and metadata
- Labeling sentiment based on likes:
  - Likes > 10 → **Positive**
  - Likes > 0 → **Neutral**
  - Likes = 0 → **Negative**

### 📊 Exploratory Data Analysis (EDA)
- Distribution of likes, text length, comment size (Big/Small)
- WordCloud for frequent terms
- Mean and max statistics per column
- Time-based sentiment trend analysis (monthly)

### 🧠 Machine Learning Pipeline
- **TF-IDF Vectorization**: Converts text into numerical features
- **Logistic Regression**: Classifier trained on labeled sentiment data
- **Label Encoding**: Converts text sentiment to integers and back
- **Model Accuracy**: Achieves 99% accuracy on test set

### 📈 Visualizations
- Bar plots of average metrics
- Pie charts of sentiment categories
- Confusion matrix heatmap
- Sentiment trendline over time using Pandas PeriodIndex

### 🧪 Model Deployment
- Model, encoder, and vectorizer saved using `joblib`
- Real-time predictions supported on new comment inputs
- Predictions include class label and probability

### 📤 Example Output:
```
Text: "I have also seen the podcast. I congratulate you both. 🎉🎉"
Predicted Sentiment: Negative
Probability: [0.9954, 0.0045]
```

---

## 🛠️ Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn, Plotly
- Scikit-learn (Logistic Regression, Label Encoding)
- WordCloud
- NLTK (stopwords, lemmatizer)
- Joblib
- Jupyter Notebook

---

## 📁 Folder Structure
```
📦 Climate_Change_Modeling
 ┣ 📜 climate_nasa.csv
 ┣ 📜 Climate_change_analysis.ipynb
 ┣ 📜 sentiment_model.pkl
 ┣ 📜 tfidf_vectorizer.pkl
 ┣ 📜 label_encoder.pkl
 ┗ 📜 README.md
```

---

## 📈 Performance Metrics

- **Accuracy**: 99.0%
- **Confusion Matrix**: Evaluated on 105 samples
```
              precision    recall  f1-score   support
           0       0.99      1.00      1.00       104
           1       0.00      0.00      0.00         1
```

> Note: Imbalance in labels due to engagement-based sentiment rule.

---

## 👩‍💻 Author
**Prajakta Koli**  
📧 koliprjkt@gmail.com  
📞 +91 9359988469  
[LinkedIn Profile](https://www.linkedin.com/in/prajaktakoli)

---

## 🙏 Acknowledgment

This project was independently developed as part of my learning journey. It enhanced my technical understanding of NLP, classification algorithms, data visualization, and real-world data interpretation — especially in the context of climate science communication.


---

