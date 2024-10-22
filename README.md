# Sentiment Analysis Project Report

### 1. Project Overview

This project involved analyzing customer reviews from a hotel dataset to extract and understand the sentiments behind customer feedback. The objective was to categorize the reviews into positive and negative sentiments, visualize the key themes using word clouds, and draw actionable insights that can help improve the hotel's customer service and operational efficiency.

### 2. Data Collection and Preprocessing

The dataset was sourced from Kaggle . 

**Link** : https://www.kaggle.com/datasets/jiashenliu/515k-hotel-reviews-data-in-europe/data

#### Key Steps:

##### Data Cleaning Stages

**Checking for Missing Values**
- Missing values were examined and addressed to ensure a complete dataset. In this case, no critical columns were dropped due to missing data.

**Converting Dates to Datetime Format**

- The Date column was converted to datetime format, enabling more accurate time-based analysis and aggregation.
  
**Feature Engineering: Extracting Month and Year**

- The month and year were extracted from the Date column and included as new features, allowing for seasonal and annual sentiment trends to be analyzed.

**Dropping Unnecessary Columns**

- Purpose: Remove columns that don't contribute to the analysis or model performance.
- The following columns were dropped to streamline the dataset:
_'Hotel_Address'_
'Additional_Number_of_Scoring'
'Average_Score'
'Hotel_Name'
'Total_Number_of_Reviews_Reviewer_Has_Given'
'Tags'
'days_since_review'
'lat'
'lng' These columns were either redundant or irrelevant to the sentiment analysis.
Exploratory Data Analysis (EDA)
Descriptive Analysis with Skimpy

Purpose: Summarize the dataset and gain insights into its structure.
Action: Skimpy was used to perform a quick and comprehensive descriptive analysis, providing statistics on numerical and categorical variables like review scores, dates, and reviewer information.
Seasonal and Annual Analysis

Purpose: Analyze how sentiments varied over different seasons and years.
Action: Sentiments were grouped by month and year to identify trends, revealing interesting seasonal patterns in review sentiments.
Distribution of Review Scores

Purpose: Understand the spread and range of review scores to evaluate general customer satisfaction.
Action: A detailed distribution analysis of the review scores was performed, showing the overall positive or negative bias in the customer reviews.
Data Cleaning: Removed duplicates, null values, and unnecessary special characters.
Text Preprocessing:
Tokenization to break the text into individual words.
Removal of stop words (common words like "the", "and", "is") that do not contribute to sentiment.
Lemmatization to reduce words to their root form (e.g., "running" to "run").
3. Sentiment Categorization
After preprocessing, the reviews were categorized into two sentiment groups:

Positive Sentiments: Reviews expressing satisfaction and praise.
Negative Sentiments: Reviews expressing complaints or dissatisfaction.
For sentiment classification, I used [mention tool/method] which accurately classified the reviews based on textual patterns and context.

4. Word Clouds for Sentiments
To visualize the most frequent words in each sentiment category, I generated two separate word clouds for positive and negative sentiments.

Positive Sentiments Word Cloud

The positive sentiment word cloud reveals key terms like "location," "great," "staff," and "breakfast." The prominence of words like "hotel" and "beautiful" indicates that customers appreciated the physical aspects and ambiance of the hotel, while "staff" and "service" suggest that customer service was a notable factor in positive feedback.

Insights from Positive Sentiments:
Top-Performing Areas:
Location: Customers frequently mentioned the convenience and attractiveness of the hotel's location.
Staff: Positive feedback about staff performance indicates strong customer service.
Breakfast & Surroundings: Amenities like breakfast and the hotel's general ambiance contributed to a positive experience.
Negative Sentiments Word Cloud

The negative sentiment word cloud highlights words such as "room," "floor," "neutral," and "angry." Complaints centered around issues with the room, possibly related to cleanliness or maintenance, as well as dissatisfaction with available facilities.

Insights from Negative Sentiments:
Improvement Areas:
Room Conditions: Words like "floor," "hot," and "dirty" suggest recurring issues with the cleanliness and comfort of rooms.
Service Issues: The mention of "angry" and "complaints" indicates customer dissatisfaction with response times or customer service quality.
5. Challenges
One of the challenges I faced during this analysis was extracting actionable insights from extremely short reviews, where sentiment might not always be clear. Another challenge was classifying neutral reviews that expressed neither strong satisfaction nor dissatisfaction. However, careful preprocessing and analysis helped mitigate these challenges.

6. Actionable Recommendations
Based on the insights drawn from the sentiment analysis, here are several actionable recommendations for improving customer experience:

Enhance Room Quality: Given the complaints about room cleanliness and temperature, it would be beneficial for the hotel to invest in improving housekeeping services and upgrading room amenities.
Improve Customer Service: While customer service was generally praised, there are still instances where customers felt frustrated. Addressing staff training and response time could help mitigate this.
Leverage Strengths: Customers appreciate the location, staff, and breakfast. The hotel can use these strengths in marketing campaigns to attract more visitors.
Targeted Feedback Collection: Introducing post-stay surveys can help the hotel gather more targeted feedback, particularly on areas that need improvement.
7. Conclusion
This project successfully identified key trends in customer feedback using sentiment analysis and word clouds. By understanding what aspects customers appreciate and where there is room for improvement, the hotel can better tailor its services to meet customer expectations, ultimately enhancing guest satisfaction and boosting repeat business.

