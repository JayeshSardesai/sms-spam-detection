# sms-spam-detection
# 📩 SMS Spam Classifier - Streamlit App

This is a simple web app that classifies SMS messages as **Spam** or **Not Spam** using Natural Language Processing and a Multinomial Naive Bayes model. It is built using Python and Streamlit.

---

## 🚀 Features

- Clean and interactive web interface (via Streamlit)
- Real-time SMS spam detection
- Uses TF-IDF for feature extraction
- Pre-trained model saved and reused for predictions

---

## 🧠 How It Works

1. The input SMS is preprocessed using NLTK:
   - Lowercasing
   - Tokenization
   - Removal of stopwords and punctuation
   - Stemming
2. The cleaned text is transformed using a saved **TF-IDF vectorizer**
3. A **Multinomial Naive Bayes** classifier predicts whether the message is spam or not

---

## 🗂️ Project Structure

sms-spam-classifier/
│<br>
├── app.py # Main Streamlit app file<br>
├── vectorizer.pkl # Saved TF-IDF vectorizer<br>
├── spam_model.pkl # Trained spam detection model<br>
└── README.md # Project documentation<br>

## Install Dependencies
Install Dependencies:

<pre> ``` pip install streamlit scikit-learn nltk ``` </pre>

Download NLTK resources:

<pre>```
import nltk
nltk.download('punkt')
nltk.download('stopwords')
 ``` 
</pre>
## Run the Streamlit App
<pre>```
streamlit run app.py  
   ```
</pre>
