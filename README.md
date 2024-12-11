# ChatGPT Reviews Analysis

## **Overview**
This project focuses on analyzing customer reviews of ChatGPT to understand user sentiment, identify trends, and gather actionable insights. Leveraging Python and data analysis libraries, it explores textual feedback to evaluate user satisfaction and highlight areas for improvement.

## **Objectives**
- Analyze customer reviews to identify sentiment trends.
- Perform text analysis to uncover key themes and common issues.
- Provide actionable insights for enhancing the ChatGPT user experience.

## **Key Features**
- **Sentiment Analysis**: Classifying reviews into positive, neutral, and negative categories.
- **Text Preprocessing**: Cleaning and tokenizing textual data for analysis.
- **Keyword Extraction**: Identifying frequently mentioned words and phrases.
- **Visualization**: Graphical representation of sentiment distribution and trends.

## **Technologies Used**
- **Python**: Primary programming language for data analysis.
- **Libraries**:
  - `Pandas` and `NumPy`: Data manipulation.
  - `Matplotlib` and `Seaborn`: Visualization.
  - `NLTK`, `TextBlob`, or `spaCy`: Text preprocessing and sentiment analysis.
  - `WordCloud`: Keyword visualization.
  - `Jupyter Notebook`: Interactive environment for coding and analysis.

## **Dataset Information**
- The dataset contains:
  - User reviews of ChatGPT.
  - Associated ratings (e.g., 1–5 stars).
  - Review timestamps.
- Describe any challenges in the dataset (e.g., imbalanced sentiment, missing ratings).

## **Steps to Reproduce**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/AnalyticJosh/ChatGPT-Reviews-Analysis.git
   cd ChatGPT-Reviews-Analysis
   ```

2. **Set Up the Environment**:
   - Install Python (3.7 or higher).
   - Install required libraries:
     ```bash
     pip install -r requirements.txt
     ```

3. **Run the Notebook**:
   - Open `ChatGPT Reviews Analysis.ipynb` in Jupyter Notebook.
   - Execute cells sequentially to preprocess data, analyze reviews, and generate insights.

## **Sample Analysis**
### Sentiment Analysis
```python
from textblob import TextBlob

def analyze_sentiment(text):
    analysis = TextBlob(text)
    if analysis.sentiment.polarity > 0:
        return 'Positive'
    elif analysis.sentiment.polarity == 0:
        return 'Neutral'
    else:
        return 'Negative'

data['Sentiment'] = data['Review'].apply(analyze_sentiment)
```

### Visualization
```python
import seaborn as sns
import matplotlib.pyplot as plt

sns.countplot(x='Sentiment', data=data)
plt.title('Sentiment Distribution')
plt.show()
```

## **Results and Insights**
- Sentiment Analysis revealed:
  - 70% positive reviews.
  - 20% neutral reviews.
  - 10% negative reviews.

## **Visualizations**
- Sentiment Distribution: Bar chart showing proportions of positive, neutral, and negative reviews.
- Word Cloud: Visualization of most frequently used terms in reviews.
- Trends Over Time: Line chart illustrating sentiment changes over review timestamps.

## **Contributions**
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

## **License**
This project is licensed under the MIT License.

---

For further inquiries or feedback, please contact [Joshua Amusan](mailto:joshuaanalyst2@gmail.com).

