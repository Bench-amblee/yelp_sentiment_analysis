# 🗣️ Yelp Sentiment Analysis 📊
## Natural Language Processing Project

![graph](/images/main_graph.jpg)
- For code go to [Notebooks](/notebooks)
- For raw data and model go to [Data](/data)
- Full [Report](Report.pdf)
- Presentation [Slides](Presentation.pdf)

**Problem Statement**

Online reviews are a common way for customers to share their thoughts on a service or product. With so much text-based data, it's impossible for a human


**Context**

This data was sourced from Yelp.com, with over 10,000 unique reviews from 200+ restaurants in New York City. The data is unlabled and will have to be classified in order to train the model. 

**Goals**

- Analyze each review and find relevant trends and relationships
- Classify the training data based on review content
- Create a prediction model with high accuracy and F1 score

**Data Collection**

Reviews were sourced from Yelp by using Yelp's Fusion API to get unique URLs for each restaurant. The list of restaurants was gathered using NYC Open Data. Using BeautifulSoup and Requests library to scrape 10,000+ reviews while following the robots.txt rules. 

![Scraping](/images/web_scraping.jpg)

**Natural Language Processing**

Each review was trimmed down by removing stop words and stemming each word. This saves memory and computing power and makes the overall model less prone to overfitting.

**Modeling**

10 models in total were tested, these are their accuracy and F1 scores:

![Model](/images/model_scores.JPG)

**Results**

Thanks to the stacked model which used features from a Sparse/Dense Matrix Naive Bayes Model and a Gradient Boosted Classifier, the overall accuracy was improved by over 20%

![Results](/images/confusion_matrices.JPG)

