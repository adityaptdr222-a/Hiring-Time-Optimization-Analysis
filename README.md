# Hiring-Time-Optimization-Analysis
Recruitment analytics dashboard using Python, pandas, seaborn, Streamlit, and Machine Learning to analyze and predict hiring time.

# Hiring Time Optimization Analysis

A recruitment analytics project built to analyze hiring data and identify delays across different stages of the recruitment process.

## About the Project

This project was built as part of an academic group project during MCA at Medi-Caps University. The goal was to analyze a recruitment dataset and find out which stages in the hiring process take the most time, and why.

We worked with a dataset of 10,000 candidate records containing details like application date, screening date, interview date, offer date, and joining date across multiple job roles and recruitment sources.

## What This Project Does

- Calculates time taken at each stage of hiring: application to screening, screening to interview, interview to offer, and offer to joining
- Compares hiring time across different job roles, recruiters, and recruitment sources
- Visualizes hiring patterns using 8 matplotlib/seaborn charts: role-wise avg hiring time, source distribution, hiring time spread (boxplot), applications per recruiter, avg hiring time by source, selected vs. rejected by role, hiring time distribution histogram, and a stage-correlation heatmap
- Shows an additional funnel chart (avg days per stage) using Streamlit's native chart
- Predicts estimated hiring time for a given role, source, and recruiter using a Linear Regression model
- Displays everything in an interactive Streamlit dashboard with filters for role, source, recruiter, and date range

## Technologies Used

- Python
- pandas for data cleaning and analysis
- matplotlib and seaborn for the 8 visualizations
- scikit-learn for the Linear Regression model
- Streamlit for the dashboard

## How to Run

Install the required libraries:

```
pip install -r requirements.txt
```

Run the app:

```
streamlit run app.py
```

Then open your browser and go to http://localhost:8501

## Dataset

The dataset (data.xlsx) contains 10,000 records with the following columns: Candidate_ID, Job_Role, Application_Date, Screening_Date, Interview_Date, Offer_Date, Joining_Date, Source, Recruiter_ID, and Status.

## Key Insights

- **Average hiring time is ~20 days** (Application to Joining) across selected candidates
- Offer-to-Join is the slowest stage on average (~10 days), longer than the first three stages combined
- Hiring time is fairly consistent across job roles and sources — no single role or source is a major bottleneck
- LinkedIn is the most-used recruitment source by volume, followed closely by Referral and Company Website
- 2,949 of 10,000 applications ended in rejection, most dropping off before the offer stage

## Author

Aditya Patidar
adityaptdr222@gmail.com
LinkedIn: https://www.linkedin.com/in/aditya-patidar03/
GitHub: https://github.com/adityaptdr222-a
