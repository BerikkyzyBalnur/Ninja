# Goodreads "Best Books Ever" Data Analysis Project

This project represents a full data science pipeline: from automated web scraping of the Goodreads website to in-depth statistical analysis and hypothesis testing.

##  Project Structure

The workflow is divided into four key phases:

### 1. Web Scraping
Using `BeautifulSoup` and `requests` to collect data on over 5,000 books. The scraper includes a logging system (`parsing_log.txt`) and features to handle rate-limiting (HTTP 429 handling, sessions, and randomized delays).

### 2. Data Cleaning & Transformation
Raw HTML data is processed into a structured `Pandas DataFrame`. This phase involves handling missing values, cleaning text fields, and converting data types for analysis.

### 3. Exploratory Data Analysis (EDA)
Analysis of rating distributions, page counts, and popular genres using:
* **Seaborn & Matplotlib**: For classic statistical plotting.
* **Plotly**: For interactive visualizations.
* **WordCloud**: To visualize frequent keywords in book titles and descriptions.

### 4. Hypothesis Testing
The project tests two main analytical theories:
* **"The Descriptor Premium"**: Investigating whether the length of a book title correlates with its average rating.
* **"Survivor Bias & Brand Loyalty"**: Analyzing the correlation between author productivity and audience loyalty.

##  How to Run

1. **Install Dependencies:**
   Ensure you have Python installed, then run the following command in your terminal:
   ```bash
   pip install -r requirements.txt
