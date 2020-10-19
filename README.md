# Data Cleaning Project: Scraping and Cleaning High-Level U.S.-Based College Data
In this Jupyter Notebook project; we scrape, compile, and clean high-level U.S. college data collected from CollegeData.com.

*Note:* Notebook file output is two separate CSV files:
- `college_data_full.csv` contains the full dataset for 1966 schools, partially cleaned and type-adjusted, but still contains missing values.  This is done to allow for availability of data for all schools, and for a user to make their own decisions about how to handle missing values based on their objectives.  Missing values are represented as:
  - `Not Reported` for string ("object") columns
  - `NaN` for numeric columns
- `college_data_ml.csv` is a filtered dataset that eliminates entries with 3 or more missing values, and uses simple column mean-based replacement for missing values.

__Required Packages__
- bs4 (BeautifulSoup)
- pandas
- numpy
