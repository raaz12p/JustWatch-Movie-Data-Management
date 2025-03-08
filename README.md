# JustWatch Movie Data Analysis

## Project Overview

This project involves web scraping movie data from [JustWatch](https://www.justwatch.com/us/movies) and analyzing the collected information. The dataset comprises 1560 movies, including details such as titles, genres, IMDb ratings, directors, runtimes, production countries, and streaming services. The goal is to explore the data through various visualizations and derive meaningful insights.

## Data Collection

### 1. Web Scraping
- **Tools Used:** `requests`, `BeautifulSoup`, `re`
- **Steps Involved:**
  1. **Get HTML Data:** Fetched the HTML content from the JustWatch movies page.
  2. **Extract Movie URLs:** Parsed the HTML to retrieve individual movie URLs.
  3. **Fetch Movie Details:** For each movie URL, extracted relevant information such as:
     - **Movie Title**
     - **Genre**
     - **IMDb Rating**
     - **IMDb Percentage**
     - **Director**
     - **Runtime**
     - **Production Country**
     - **Streaming Service**

### 2. Data Cleaning and Preprocessing
- Cleaned the scraped data by handling missing values, normalizing genres, and converting runtimes into a uniform format.
- Parsed IMDb ratings and percentages to numerical values for analysis.

### 3. DataFrame Creation
- Consolidated all the cleaned data into a Pandas DataFrame.
- Columns include:
  - `Movie Title`
  - `Genre`
  - `IMDb Rating`
  - `IMDb Percentage`
  - `Director`
  - `Runtime`
  - `Production Country`
  - `Streaming Service`

## Data Visualization

Various charts and plots were created to visualize the data and uncover patterns:

### 1. Bar Chart
- **Purpose:** Shows the count of movies per genre.
- **Insight:** Identifies the most and least common genres in the dataset.

### 2. Histogram
- **Purpose:** Displays the distribution of IMDb ratings.
- **Insight:** Highlights the concentration of ratings and identifies any skewness in the data.

### 3. Box Plot with Violin Plot Overlay
- **Purpose:** Combines a box plot with a violin plot to show the distribution of IMDb ratings across genres.
- **Insight:** Provides a detailed view of the spread and density of ratings.

### 4. Facet Grid with Histograms
- **Purpose:** Faceted histograms showing the distribution of IMDb ratings across different production countries.
- **Insight:** Compares how ratings vary across different regions.

### 5. Heatmap
- **Purpose:** Heatmap of Genre vs. IMDb Rating.
- **Insight:** Reveals correlations between specific genres and rating levels.

### 6. Pair Plot
- **Purpose:** Visualizes relationships between numeric features such as IMDb rating, runtime, and percentage.
- **Insight:** Identifies potential correlations and patterns between different variables.

### 7. Interactive Scatter Plot with Plotly
- **Purpose:** An interactive scatter plot allowing users to explore the relationship between IMDb ratings and runtime, filtered by genre.
- **Insight:** Offers a dynamic way to investigate trends in the data.

## How to Use

### Prerequisites
- Python 3.x
- Install necessary libraries using:
  ```bash
  pip install requests beautifulsoup4 pandas numpy matplotlib seaborn plotly
  ```

### Running the Project
1. **Scrape Data:** Run the script to scrape movie data from JustWatch.
2. **Analyze Data:** Use the provided notebooks or scripts to analyze the data and create visualizations.
3. **Explore Visualizations:** Open the interactive Plotly charts to explore the data in detail.

## Conclusion

This project demonstrates how web scraping can be leveraged to gather and analyze real-world data. Through various visualizations, the project uncovers patterns in movie genres, ratings, and more. The insights derived can be valuable for understanding trends in the film industry.

## Future Work
- Expand the dataset by scraping additional pages or other regions.
- Perform sentiment analysis on movie reviews.
- Apply machine learning models to predict movie ratings based on other features.

## Data Visualizations

### 1. Showing the Count of Movies per Genre
![Bar Chart](1_Showing%20the%20count%20of%20movies%20per%20genre.png)

### 2. Distribution of IMDb Ratings
![Bar Chart](2_Distribution%20of%20IMDb%20ratings.png)

### 3. Facet Grid with Histograms
![Bar Chart](4%20Facet%20Grid%20with%20Histograms.png)

### 4. Pair Plot of Numeric Features
![Bar Chart](6%20Pair%20Plot%20of%20Numeric%20Features.png)




