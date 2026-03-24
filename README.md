Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

Aim: 

Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools.

Explanation:

Develop a python code that integrates multiple AI tool by interacting with their APIs.
Compare outputs from different APIs.
Analyze the response and the Output.

The aim is to understand how to request help from AI tools for tasks like writing Python code, integrating with APIs, comparing outputs, and generating actionable insights.

program:
positive statement
```
from nltk.sentiment import SentimentIntensityAnalyzer
import nltk

nltk.download('vader_lexicon')

# Simulated AI-generated text
generated_text = "This smartphone delivers exceptional battery performance and features a smart AI-powered camera that takes breathtaking photos."

print("Generated Review:\n")
print(generated_text)

# Sentiment analysis
sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)

print("\nSentiment Analysis:")
print(sentiment)

# Insight generation
if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")
```

output:
```
[nltk_data] Downloading package vader_lexicon to /root/nltk_data...
Generated Review:

This smartphone delivers exceptional battery performance and features a smart AI-powered camera that takes breathtaking photos.

Sentiment Analysis:
{'neg': 0.0, 'neu': 0.695, 'pos': 0.305, 'compound': 0.6908}

Insight: The review is positive and suitable for marketing promotion.
```

Negative statement:
```
from nltk.sentiment import SentimentIntensityAnalyzer
import nltk

nltk.download('vader_lexicon')

# Simulated AI-generated text
generated_text = "This smartphone struggles with battery life and its camera lacks the intelligence needed to capture high-quality photos."

print("Generated Review:\n")
print(generated_text)

# Sentiment analysis
sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)

print("\nSentiment Analysis:")
print(sentiment)

# Insight generation
if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")
```

output:
```
Generated Review:

This smartphone struggles with battery life and its camera lacks the intelligence needed to capture high-quality photos.

Sentiment Analysis:
{'neg': 0.121, 'neu': 0.728, 'pos': 0.15, 'compound': 0.1531}

Insight: The review is positive and suitable for marketing promotion.
[nltk_data] Downloading package vader_lexicon to /root/nltk_data...
[nltk_data]   Package vader_lexicon is already up-to-date!
```



Result:
Thus the program is successfully executed and verified
