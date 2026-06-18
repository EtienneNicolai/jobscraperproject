Australian AI & Data Job Market Analysis Overview

This project was developed as part of my effort to improve practical machine learning, NLP, and data engineering skills by analysing real world Australian job market data using Adzuna API.

This project was originally going to be an analysis of the skills required for certain fields and then use machine learning to find the best combination, however about mid way through the project I learned the API I was using only pulled up to 500 characters of the job description severely limiting the project. Thus I changed the project to analyze Australian technology job listings and identify hiring trends, geographic demand, and common job categories within the AI, data science, analytics, and software engineering job market. additionally the search terms can be changed to suit field

The project combines data collection, data cleaning, exploratory analysis, natural language processing (NLP), and machine learning clustering techniques.


Features:
Collects live australian job listings from the Adzuna API
Search across multiple related job categories
Clean and normalize job location data
Analyzes jobs by location
Performs NLP preprocessing using TF-IDF
Uses KMeans clustering to identify job categories
Groups similar roles into meaningful market segments

The following search terms are used:
data scientist
machine learning engineer
ai engineer
data analyst
software engineer
data engineer
business analyst

Technologies Used
Python
Pandas
Requests
Scikit-learn
Jupyter Notebook
Git/GitHub



Project Workflow
Adzuna API -> Job Collection -> Data Cleaning -> Location Normalization -> Exploratory Analysis -> TF-IDF Feature Extraction -> K-Means Clustering -> Machine Learning Approach


K-Means clustering is used to group similar job listings based on textual similarity.
The model identifies several distinct categories including:

AI / Machine Learning Engineering
Software Engineering
Data Science & Analytics
Industry & Specialist Analytics
Business Analytics
Key Findings
Geographic Demand

The highest concentration of technology roles was found in:
Melbourne and Sydney



Limitations 
Adzuna provides job descriptions truncated to approximately 500 characters. This prevented my original plan of analysing the skills demanded in each job (python, C# etc) so I pivoted to Role/location/market classification rather than detailed skill extraction.

Future Improvements
Collect more data.
Could add visualizations for cluster exploration.
Perform seniority analysis (Graduate, Junior, Senior, Lead).
Build an interactive dashboard using Streamlit.
Integrate additional job data sources.
use alternative API for longer descriptions and analyse skills.

To replicate this have the project under this structure
jobscraperproject/
│
├── data/
│   └── raw/
│       └── jobs.csv
│
├── jobscraperproject.ipynb
├── config.py          (excluded from Git) ---> this file should contain your own Adzuna API and Key
├── .gitignore
└── README.md