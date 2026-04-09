# AirBnB Listing Analysis Using Python

![Python](https://img.shields.io/badge/Python-Data%20Analysis-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

## Project Overview
This project analyses **Airbnb listings data** to uncover insights about **pricing, neighbourhood trends, accommodation capacity, and host growth over time in Paris**.

Using **Python and data analysis libraries**, the project explores the dataset, performs data quality checks, prepares aggregated tables, and creates visualisations to better understand the Airbnb market in Paris.

The workflow includes **data exploration, transformation, and visualisation** to answer key business questions.

---

# Resource

Download the [dataset](https://drive.google.com/file/d/1iAbKh-olyOM6uTUgXBwEZE2_545Mhh_5/view?usp=sharing "Listings.csv")

---

# Objectives

## 1. Data Exploration & Quality Assessment
The first phase focuses on understanding the dataset and identifying potential quality issues.

Key steps include:

- Importing the dataset using **Pandas**
- Converting the `host_since` column into **datetime format**
- Filtering the dataset to include only **Paris listings**
- Selecting relevant columns:
  - `host_since`
  - `neighbourhood`
  - `city`
  - `accommodates`
  - `price`
- Performing **data quality checks**
  - Checking for missing values
  - Computing minimum, maximum, and average values for numeric columns

---

## 2. Data Preparation
To support analysis and visualisation, the dataset is transformed into summary tables.

### Neighbourhood Pricing Analysis

A table called:

`paris_listings_neighbourhood`

This table:

- Groups listings by **neighbourhood**
- Calculates the **average price per neighbourhood**
- Sorts neighbourhoods by **highest average price**

---

### Accommodation Pricing Analysis

A second table called:

`paris_listing_accommodates`

This table:

- Filters the dataset to the **most expensive neighbourhood**
- Groups listings by **number of guests accommodated**
- Calculates the **average price for each accommodation size**

---

### Host Growth Over Time

A third table called:

`paris_listings_over_time`

This table groups listings by the **year hosts joined Airbnb** and calculates:

- **Number of new hosts per year**
- **Average listing price per year**

---

# Data Visualisations

The project produces several charts to communicate insights clearly.

### 1. Average Price by Neighbourhood

A **horizontal bar chart** showing:

- Average Airbnb price across neighbourhoods in Paris
- Comparison of high-value and lower-value locations

---

### 2. Price vs Accommodation Size

A **horizontal bar chart** illustrating:

- The relationship between **price and number of guests accommodated**

---

### 3. Host Growth vs Price Over Time

A **dual-axes chart** displaying:

- **New Airbnb hosts joining per year**
- **Average listing price over time**

This visualisation highlights **how platform growth correlates with pricing trends**.

---

# Technologies Used

- **Python**
- **Pandas** – Data manipulation and analysis
- **Seaborn** and **Matplotlib** – Data visualisation
- **Jupyter Notebook** – Interactive analysis environment
