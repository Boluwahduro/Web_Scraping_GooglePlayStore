# Web_Scraping_GooglePlayStore for Spotify Reviews
**Overview:**
This project aimed to scrape reviews of the Spotify app from the Google Play Store, focusing on Spotify's top global markets across North America, Latin America, Asia, and Africa. The countries selected for this analysis included the United States, Canada, the United Kingdom, Ireland, Sweden, Mexico, Spain, the Philippines, India, Nigeria, South Africa, Ghana, and Kenya.

**Key Highlights:**
**Scraping:** The google_play_scraper library was used to fetch all the reviews for the selected countries from the Google Play Store.
**Data Cleaning:**
**Duplicates:** The dataset was processed to remove duplicate entries based on the combination of 'userName' and 'content'. This was done in chunks to handle large datasets without memory issues. Any remaining duplicates were removed after the chunk-wise processing.
**Missing Values**: Missing values in the 'appVersion' column were replaced with 'unknown'.
**Date Formatting:** The 'date' column was converted to datetime format.
**File Management:** The scraped reviews were saved after each country's data was fetched to ensure data persistence in case of any interruptions. The cleaned dataset was saved as 'google_play_reviews22.csv'.
**Analysis:** The final cleaned dataset was examined to get insights such as the date range of the reviews and the number of reviews per country.

**Results:**
The cleaned dataset provided a comprehensive view of Spotify's reviews across the selected countries, starting from the earliest review date to the latest in 2023. This dataset can be further used for sentiment analysis, trend analysis, and more.

**Future Scope:**
Sentiment Analysis: Understand the sentiment behind the reviews and possibly correlate with app versions or specific events.
Trend Analysis: Observe if there are any patterns or trends in reviews over time.
Expand to other apps: The methodology used here can be applied to other apps to compare and contrast user feedback.

**Repository Contents:**
google_play_reviews.csv: Initial scraped data.
google_play_reviews_filtered.csv: Data post chunk-wise duplicate removal.
google_play_reviews22.csv: Final cleaned dataset.
Script: Contains the Python code for scraping, cleaning, and data manipulation.


Note: Always ensure you have the necessary permissions and adhere to terms of service when scraping data from websites or platforms.
