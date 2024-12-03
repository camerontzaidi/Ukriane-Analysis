Conflict Analysis Project Repository

Overview

Welcome to the “Conflict Analysis” project repository. This project provides an in-depth analysis of the Russia-Ukraine conflict, focusing on arms transfers, conflict events, and media reporting. By integrating diverse data sources and applying advanced analysis techniques, this project uncovers key insights about the geopolitical, military, and media dynamics of the ongoing conflict.

Repository Structure

conflict-analysis/
│
├── 141B_project.ipynb          # Jupyter Notebook with all analysis, code, and visualizations
├── data/                       # Folder containing preprocessed datasets
│   ├── acled_data.csv          # Cleaned ACLED event data
│   ├── sipri_ukraine.csv       # SIPRI arms transfer data for Ukraine
│   ├── sipri_russia.csv        # SIPRI arms transfer data for Russia
│   ├── cnn_fox_articles.csv    # Web-scraped articles from CNN and Fox News
├── README.md                   # Project overview and instructions
└── LICENSE                     # Licensing information

Data Sources

	1.	ACLED (Armed Conflict Location & Event Data Project)
	•	Provides detailed conflict event data, including event type, location, and dates.
	•	Accessed via ACLED’s API with custom parameters.
	2.	SIPRI (Stockholm International Peace Research Institute)
	•	Contains data on global arms transfers to Ukraine and Russia.
	•	Manually downloaded due to the absence of API support.
	3.	CNN and Fox News Articles
	•	Web-scraped using Selenium and BeautifulSoup.
	•	Keyword analysis performed to study media sentiment and focus.

Key Features

Data Acquisition

	•	ACLED API:
Accessed using Python scripts, with parameters to filter data by region, event type, and date.
	•	SIPRI Data:
Processed manually due to the lack of an API. Data cleaning and merging were done to ensure consistency.
	•	Web Scraping:
Articles from CNN and Fox News were extracted using Selenium to navigate dynamic web pages and BeautifulSoup to parse HTML.

Exploratory Data Analysis (EDA)

	•	Visualization of arms transfers to Ukraine and Russia by weapon type and supplier.
	•	Time-series plots of conflict intensity and event types from 2022 to 2024.
	•	Keyword frequency trends in CNN and Fox News reporting.

Insights

	•	Identified the dominance of the United States in supplying weapons to Ukraine.
	•	Highlighted the increasing frequency of battles and drone strikes over time.
	•	Unveiled differences in media focus, with CNN emphasizing technological warfare (e.g., drones) and Fox News focusing on geopolitical narratives.

Usage Instructions

	1.	Clone the Repository
Clone this repository to your local machine:

git clone https://github.com/your-repo-link
cd conflict-analysis


	2.	Dependencies
Install the required Python libraries:

pip install -r requirements.txt


	3.	Run the Notebook
Open and execute the Jupyter Notebook to reproduce the analysis:

jupyter notebook 141B_project.ipynb


	4.	Explore the Data
All preprocessed datasets are located in the data/ folder and are ready for further analysis.

Challenges and Solutions

Challenges

	•	SIPRI Data:
Manual data acquisition introduced workflow complexity due to the lack of API.
	•	ACLED Bias:
Event underreporting and potential bias from media sources posed challenges in data interpretation.
	•	Web Scraping:
Dynamic web pages on CNN and Fox News required Selenium to bypass JavaScript-rendered content.

Solutions

	•	Automated processes for repetitive data acquisition tasks.
	•	Emphasized data cleaning and error handling to ensure reliability.
	•	Adjusted scraping techniques to handle dynamic web elements effectively.

Acknowledgments

	•	ACLED for conflict event data: ACLED Website
	•	SIPRI for arms transfer data: SIPRI Website
	•	CNN and Fox News for media articles.

