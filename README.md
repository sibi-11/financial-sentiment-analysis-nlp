# Financial News Sentiment Analysis using NLP

This project demonstrates the application of Natural Language Processing (NLP) and Transformer models to analyze the sentiment of financial news headlines. The goal is to classify news as `positive`, `negative`, or `neutral` to potentially aid in investment research and decision-making.

## 🚀 Skills Demonstrated

- **Natural Language Processing (NLP)**: Using state-of-the-art transformer models for text classification.
- **Hugging Face Transformers**: Leveraging the `transformers` library to use a pre-trained model fine-tuned on financial news.
- **Data Analysis & Visualization**: Using `pandas`, `matplotlib`, and `seaborn` to analyze and visualize results.
- **Domain Application**: Applying AI to the financial domain.

## 📁 Project Structure

financial-sentiment-analysis-nlp/
├── financial_sentiment_analysis.ipynb # Main Jupyter notebook
├── all-data.csv # Input dataset (from Kaggle)
├── financial_news_sentiment_predictions.csv # Output results
├── sentiment_analysis_results.png # Output visualization
└── README.md

## 📊 Dataset

The dataset used is **Sentiment Analysis for Financial News** from Kaggle.
- **Source**: [Kaggle Link](https://www.kaggle.com/datasets/ankurzing/sentiment-analysis-for-financial-news)
- It contains over 4800 headlines labeled as `positive`, `negative`, or `neutral`.

## ⚙️ Implementation

1.  **Data Loading**: The financial news dataset is loaded and prepared.
2.  **Model**: Used a pre-trained DistilRoBERTa model (`mrm8488/distilroberta-finetuned-financial-news-sentiment-analysis`) from Hugging Face, specifically fine-tuned for financial news sentiment.
3.  **Analysis**: The model's pipeline is used to predict the sentiment of a sample of headlines.
4.  **Evaluation & Visualization**: Results are compared to ground-truth labels (where available), and the distribution of sentiments and model confidence is visualized.

## 📈 Results

The model successfully classifies sentiments with high confidence. The visualization includes:
- A count plot showing the distribution of predicted sentiments.
- A bar plot showing the average confidence level for each sentiment class.

![Sentiment Analysis Results](sentiment_analysis_results.png)

## 🛠️ How to Run

1.  Clone the repository.
2.  Install dependencies: `pip install transformers pandas numpy matplotlib seaborn`
3.  Download the dataset from Kaggle and place `all-data.csv` in the project folder.
4.  Run the Jupyter notebook `financial_sentiment_analysis.ipynb`.

## 🔮 Future Work

- Integrate this analysis with a live financial news API.
- Build a dashboard for real-time sentiment tracking.
- Explore the correlation between news sentiment and stock price movements.

