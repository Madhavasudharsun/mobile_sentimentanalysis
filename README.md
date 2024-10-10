# mobile_sentimentanalysis
1.Web Scraping Reviews:

Set up Selenium WebDriver to navigate Flipkart product pages.
Extract product reviews, ratings, and titles using class selectors.
Paginate through reviews using the "Next" button.
Save the scraped reviews (mobile name, rating, title, content) into a list.

2.Data Cleaning:
Clean review content by removing redundant terms such as "purchase" and "read more."
Handle missing data by dropping incomplete records.
Save the cleaned data to a CSV file (flipkart_review.csv).

3.Sentiment Analysis:
Use TextBlob to calculate polarity scores for each review.
Classify reviews into positive, negative, or neutral based on polarity scores.
Adjust sentiment based on the star rating and polarity score (e.g., 3+ stars with positive polarity considered positive).

4.Mobile Recommendation:
Group reviews by mobile model and calculate the average sentiment score.
Sort mobile phones by sentiment to identify the top-rated phone.
Use LangChain to generate a recommendation for the top mobile phone based on user sentiment.

5.Saving Results:
Save the sentiment analysis results to a CSV file (sentiment_analysis.csv).
Print the final mobile recommendation using a LangChain template.

6.Streamlit Application:
Load the LangChain recommendations from the pickle file.
Add additional data for price and brand.
Create an interactive Streamlit app with filters for brand and price range.
Display mobile recommendations with images and key details like positive review count and price.

7.Deployment on AWS:
Deploy the Streamlit app on AWS.
Ensure that necessary libraries like Streamlit, Pandas, Pickle, Requests, and PIL are installed.
Set up the AWS environment to serve the application.
