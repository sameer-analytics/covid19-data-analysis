#Covid-19 Country wise Data Analysis Repository

This repository contains two key folders:  
1. **covid-19 data analysis complete portfolio**  
2. **covid-19 data analysis full project**  

Each folder serves a specific purpose to present and analyze the scrapped data .

---

## Folder Structure

### 1.covid-19 data analysis complete portfolio 
This folder contains curated content for showcasing the analysis of covid-19 data both country and region wise. It highlights key insights and visualizations derived from the analysis.

- **Contents:**
  - **01_data:**  
    - **01_data_source.txt** This file contains the website link from where i have scrapped data
    - **02_Covid-19 countrywise cleand dataset.csv** This is the cleaned data set of this project with csv format 

  - **02_scripts:**  
    Python scripts for the analysis workflow:  
    - **a_required_library_imports.ipynb** common Library imports.  
    - **b_data_collection(web scrap).ipynb** It contains the code for webscraping the data from the website and cleaning part of raw data to convert a dataframe   
    - **c_data_exploration.ipynb** It contains exploration of the project
    - **d_data_cleaning.ipynb** It contains the cleaning part of the data   
    - **e_explorartory_data_analysis(EDA).ipynb:** Exploratory Data Analysis.  
    - **insights_code.ipynb** It contains the project insights code
    - **country_wise_covid-19_data analysis dashboard.pbix** This contains the powerBI visualizations Dashboards

  - **03_output:**  
    - **a_visualizations(dashboard_images):** This is the folder which contains the png files of  dashboard images   
    - **b_report:**This folder containas the insights.md file summarizing insights and findings.  

  - **README.md:** Documentation describing the folder content and analysis steps.  
  - **requirements.txt:** all libraries required to execute the scripts.

---

### 2.covid-19 data analysis full project
This folder contains the complete project workflow, starting database connection to generating insights. It serves as a detailed analysis pipeline for the analysis.  

- **Contents:**
  - **a_data**    
    - **a_data_source.txt** This file contains the url link from where i have scrapped the data.

  - **b_complete_project**  
    Includes the Python script that performs the entire data analysis workflow.  
    - **full_project.ipynb** The script covers:
      - Importing libraries.
      - Data Collection using Web Scraping.
      - Data exploration.
      - Data Cleaning
      - Exploratory Data Analysis (EDA).
      - Insights and recommendations.
    - **country_wise_covid-19_data analysis dashboard using powerBI.pbix**: this is the powerBI files which contains the project Dashboards

---

## Technologies Used

- **Programming Language:** Python  
- **Libraries:** pandas, numpy, matplotlib, seaborn, regular expression ,BeautifulSoup ,requests
- **visualization tool:** PowerBI 
- **Development Environment:** jupyter notebook  
- **Dataset Format:** csv 

---

## Project Highlights

1. **Data Source Overview:**
   - the link from where i have scrapped the data contains the table which have the columns like country ,region , cases, death

2. **Key Steps:**
   - Data Collection: Using BeautifulSoup I have collected the data and cleaned the raw data and make the data frame from the website
   - library imports: imported all the required libraries
   - Data Exploration: I have done the exploration part using pandas
   - Data Cleaning: i have done the cleaning using re and pandas.
   - Exploratory Data Analysis (EDA): Perfomed the EDA using both code and visual
   - Visualizations: created interactive dashboards using piwerBI.
   - Insights and Recommendations: Actionable strategies derived from the analysis.

3. **Portfolio Content:**  
   A focused summary of the analysis, including visualizations and insights for easy understanding and presentation.

4. **Full Project Content:**  
   Detailed workflow showcasing the complete analysis pipeline from raw data to insights.

---

## Contact Information

- **Name:** Sameer Nayak  
- **Email:** sameernayak6370@gmail.com  
- **LinkedIn:** [Sameer Nayak LinkedIn](https://www.linkedin.com/in/sameer-nayak-5a147a260/overlay/about-this-profile/?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base%3ByaSYCprkSPi72GIGsfx7UA%3D%3D)  
- **Portfolio:** [GitHub Portfolio](https://github.com/sameer-analytics/covid19-data-analysis)  
