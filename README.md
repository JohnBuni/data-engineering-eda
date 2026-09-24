# Data Engineering & EDA Workshop

This project demonstrates an end-to-end data engineering and exploratory data analysis (EDA) workflow using Python, PostgreSQL, and Pandas.

## Project Overview

The project generates a synthetic employee dataset containing 50 employees with IT-related job positions, start dates, and salaries. The employee data is stored in a cloud PostgreSQL database hosted on Neon and then retrieved into Python for analysis.

The notebook demonstrates:

- Synthetic data generation using Faker
- Cloud PostgreSQL database storage using Neon
- Database connectivity using psycopg2
- Data manipulation and analysis using Pandas
- Data cleaning and descriptive statistics
- Feature engineering
- Salary standardization using scikit-learn
- Data visualization using Matplotlib and Seaborn
- Dataset merging using additional department information
- Grouped bar chart and heatmap visualizations

## Technologies Used

- Python
- Jupyter Notebook
- PostgreSQL
- Neon
- Pandas
- Faker
- psycopg2
- scikit-learn
- Matplotlib
- Seaborn

## Files

`data_engineering_eda.ipynb` — Main Jupyter Notebook containing the complete data engineering workflow, EDA, and visualizations.

`.gitignore` — Prevents local environment files and database credentials from being committed to the repository.

## Database Security

The PostgreSQL connection string is stored locally in a `.env` file and is intentionally excluded from this repository to protect database credentials.