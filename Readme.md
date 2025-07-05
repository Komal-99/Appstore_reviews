App Store Reviews Scraper

This project scrapes user reviews for the app from the Apple App Store across multiple countries, processes the data, and exports it to a CSV file for further analysis.

## Features

- Scrapes reviews from the Apple App Store using the `app-store-web-scraper` package.
- Supports multiple country codes (e.g., US, IN, GB, CA, AU, AE, DE, FR, IT, SG).
- Cleans and filters review data to remove sensitive customer information.
- Converts the reviews into a structured pandas DataFrame.
- Exports the cleaned data to appstore_reviews.csv.

## Requirements

- Python 3.11+
- Packages:
  - requests
  - pandas
  - tqdm
  - numpy
  - app-store-web-scraper

## Installation

Install the required packages using pip:
```
pip install requests pandas tqdm numpy app-store-web-scraper
```


## Usage

1. Open and run the Jupyter notebook scrape_app_store_reivews.ipynb.
2. The notebook will:
   - Fetch reviews for the app from the App Store for each country in the list.
   - Remove sensitive fields (`user_name`, `id`).
   - Convert the reviews to a pandas DataFrame.
   - Save the DataFrame to appstore_reviews.csv.

## Output

- The final output is a CSV file: appstore_reviews.csv, containing the following columns:
  - `content`
  - `score`
  - `at`
  - `title`
  - `reviewCreatedVersion`
  - `Country`
  - `replyContent`
  - `repliedAt`

## Notes

- The notebook is designed for exploratory data analysis and can be extended for further processing or visualization.
- Make sure your IP address is not rate-limited by the App Store when running the scraper for multiple countries.

---

For any questions or issues, please refer to the code in scrape_app_store_reivews.ipynb.
