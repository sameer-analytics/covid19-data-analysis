## COVID-19 Web Scraping and Data Analysis

### Project Description
This project involves web scraping COVID-19 data from Worldometer and performing data analysis to uncover insights related to cases, deaths, and mortality rates. The analysis covers data cleaning, exploratory data analysis (EDA), and visualization to derive meaningful insights about the impact of COVID-19 across different regions and countries.

---

### Data Collection

- **Source:** Worldometer - Countries Where COVID-19 Has Spread
- **Method:** Web scraping using the `requests` library and `BeautifulSoup` to extract tabular data from the webpage.
- **Data Extracted:**
  - **Country:** Name of the country.
  - **Cases:** Total reported cases in the country.
  - **Deaths:** Total reported deaths in the country.
  - **Region:** Geographical region of the country.

---

## *Steps Performed*

### 1.Importing Required Libraries

**Libraries Used:**
- `numpy`: For numerical computations.
- `pandas`: For data manipulation and analysis.
- `matplotlib.pyplot`: For data visualization.
- `seaborn`: For enhanced visual representation of data.
- `re`: For regular expression-based data cleaning.
- `BeautifulSoup`: For web scraping.
- `requests`: For making HTTP requests to fetch data from the website.

### 2. Web Scraping and Data Extraction

**Performed Actions:**
- Sent an HTTP request to the website to fetch data.
- Parsed the HTML content using `BeautifulSoup`.
- Extracted tabular data using `findAll("td")`.
- Cleaned extracted data using `re.sub()`.
- Stored data into lists and created a structured `DataFrame` using `pandas`.

### 3. Data Exploration

**Actions Performed:**
- Displayed the first and last 5 rows of the dataset.
- Checked the shape of the dataset.
- Checked for missing values.
- Identified unique values in categorical columns.
- Checked data types and performed data type conversions.
- Counted duplicate entries.

### 4. Data Cleaning

**Performed Actions:**
- Handled hidden string values in the `region` column.
- Replaced missing or whitespace values with "no region".
- Removed thousands separators from numerical columns and converted them to `int`.
- Added a new column `mortality_rate` calculated as `(deaths/cases) * 100`.
- Sorted the dataset by the number of cases in descending order.
- Replaced infinite and scientific notation values with appropriate numbers.
- Rounded off `mortality_rate` values to 2 decimal places.

### 5. Exploratory Data Analysis (EDA)

**Summary Statistics:**
- Generated descriptive statistics for numerical columns.

**Outlier Detection:**
- Used boxplots to detect outliers in `cases`, `deaths`, and `mortality_rate`.

**Distribution Analysis:**
- Used histograms to visualize distributions of `cases`, `deaths`, and `mortality_rate`.

**Correlation Analysis:**
- Used scatter plots to analyze the correlation between `cases` and `deaths`.

**Regional Summary:**
- Aggregated `cases` and `deaths` by `region` to identify trends.

**Top 10 Countries Analysis:**
- Identified the top 10 countries by `cases`, `deaths`, and `mortality_rate`.

### 6.Data Visualizations
- Created a dashboard of this project using powerBI

---

## *Key Insights*

### 1. Countries with Highest Cases and Deaths
- The **United States, India, and France** have the highest number of cases.
- The **United States** also leads in deaths, followed by **Brazil** and **India**.
- **Recommendation:** Analyze healthcare policies and pandemic management strategies in these countries to identify best practices.

### 2. Highest and Lowest Mortality Rates
- **North Korea, Nauru, and Cook Islands** have the highest mortality rates.
- **Falkland Islands, Holy See, and Tokelau** report a 0.0 mortality rate.
- **Recommendation:** Improve healthcare infrastructure in high-mortality countries and review data accuracy for low-mortality ones.

### 3. Correlation Between Cases and Deaths
- Strong **positive correlation (0.8863)** between cases and deaths.
- **Recommendation:** Strengthen healthcare systems in high-case regions to reduce fatality rates.

### 4.Regional Impact of COVID-19
- **Europe** has the highest number of cases and deaths.
- The **"no region" category** has very low cases, indicating potential data gaps.
- **Recommendation:** Address data inconsistencies and enhance pandemic preparedness in high-case regions.

### 5. Outlier Detection in Deaths**
- Few countries report exceptionally high deaths, appearing as **outliers**.
- **Recommendation:** Improve healthcare access and response mechanisms in high-mortality regions.

---

## *Technologies Used*

- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, BeautifulSoup, Requests
- **Tool**: powerBI
- **Development Environment:** Jupyter Notebook 
- **Dataset Format:** Web-scraped data stored in CSV format

---

## *Folder Structure*

### *01_data*
- 01_data_source.txt: Contains the web scraping website link.
- 02_Covid-19_countrywise_data.csv: CSV file storing country-wise COVID-19 data.

### *02_scripts*
- a_required_library_setup.ipynb: Jupyter notebook for setting up necessary libraries.
- b_data_collection_web_scraping.ipynb: Notebook performing web scraping to collect data.
- c_data_exploration.ipynb: Notebook analyzing dataset structure and summary statistics.
- d_data_cleaning.ipynb: Notebook handling missing values and data inconsistencies.
- e_exploratory_data_analysis.ipynb: Notebook performing visual analysis and insights generation.
- insights_code.ipynb: Notebook compiling findings and generating key insights.
- country_wise_covid-19_data analysis dashboard.pbix:This file has the dashboard of the project

### *03_output*
- **a_visualizations(dashboard_images):**
      - covid-19 country wise data analysis dashboard.png :This is the image of the dashboard
- **b_reports**
      - insights.md: It contains the summerize of the insights
  
**README.md:** Documentation describing the project overview, steps, and insights.
**requirements.txt:** Lists all the libraries required to run the project.
