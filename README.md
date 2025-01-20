# 🎬 Movie Review Analysis 🍿

## 📝 Project Overview
This is a Streamlit-based web application that uses a pre-trained deep learning model to analyze the sentiment of movie reviews. The application classifies movie reviews as either Positive or Negative using a machine learning model trained on the IMDB dataset.

## 🛠️ Requirements
1. numpy
2. pandas
3. tensorflow
4. scikit-learn
5. streamlit
6. tensorboard

## 💾 Installation

1. Clone the repository:
```cmd
git clone https://github.com/Yuvraj0014/Sentiment-Analysis-using-RNN-and-NLP.git
cd Sentiment-Analysis-using-RNN-and-NLP
```

2. Setup a virtual environment (optional but recommended)
```cmd
python -m venv venv
source venv/bin/activate  # For Linux/MacOS
venv\Scripts\activate  # For Windows
```

3. Install required dependencies
```cmd
pip install -r requirements.txt
```

4. Run the streamlit app
```cmd
streamlit run app.py
```

## Results 
```
review-analysis-using-rnn.streamlit.app
```

## 🔍 How to Use the Application
1. Open the web application in your browser 💻
2. Navigate to the sidebar 👉
3. Enter a movie review in the text area ✍️
4. Click "Classify Sentiment" button 🏁
5. View the sentiment prediction and score 📊

## 📈 Output Prediction
### Classification Mechanism 🧠
The sentiment classification is based on a neural network model trained on the IMDB dataset, which uses a probabilistic approach:

- **Prediction Score Range**: 0 to 1
- **Positive Sentiment** 😄: Score > 0.5
- **Negative Sentiment** 😞: Score ≤ 0.5

### How Classification Works
1. **Text Preprocessing**:
   - Convert input to lowercase
   - Tokenize the review into words
   - Map words to numerical indices
   - Pad the sequence to a fixed length (500 words)

2. **Model Prediction**:
   - Input processed text into pre-trained neural network
   - Model generates a probability score between 0 and 1
   - Closer to 1 indicates more positive sentiment
   - Closer to 0 indicates more negative sentiment

3. **Decision Boundary**:
   - Score > 0.5: Classified as Positive Review
   - Score ≤ 0.5: Classified as Negative Review

**Example**:
- Review Score 0.75 → Positive Sentiment 😃
- Review Score 0.45 → Negative Sentiment 😔

### Confidence Interpretation
- Scores near 0.5 indicate uncertain or neutral sentiment
- Scores further from 0.5 (closer to 0 or 1) show stronger sentiment confidence

## 🖥️ Application Interface
- Centered layout with a cinema-themed design 🎥
- Sidebar for review input and sentiment analysis 📋
- Color-coded sentiment display 🌈
- Informative tips and instructions 💡

## Output Screen
![Screenshot 2025-01-20 203155](https://github.com/user-attachments/assets/5929afc9-b700-45f4-b95b-70ca26c297ee)


## 📌 Note
Ensure you have the pre-trained model (`simple_rnn_imdb.h5`) in the same directory before running the application. 🔍
