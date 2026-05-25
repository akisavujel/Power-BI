# Patient Data Analysis Dashboard

A Power BI dashboard project focused on analyzing patient demographic data. This project demonstrates data cleaning, transformation, and visualization techniques using Power BI.

## Project Overview

The goal of this project was to clean and transform raw patient data and build an interactive dashboard to visualize population insights such as gender distribution, marital status, ethnicity, and birth trends.

## Dataset Cleaning & Transformation

The following data preparation steps were performed in Power BI Power Query:

- Connected to the patient data CSV file
- Verified and corrected data types
- Removed unnecessary columns:
  - `LAT`
  - `LON`
  - `SUFFIX`
  - `STATE`
- Filled missing values in:
  - `ZIP`
  - `MARITAL`
- Created a custom column called `Status`
  - `Alive` if `DEATHDATE` is null
  - `Deceased` otherwise
- Extracted birth year from the `BIRTHDATE` column
- Verified data types for newly created columns

## Dashboard Features

The dashboard includes the following visualizations:

- **Card Visual**
  - Total Population measure

- **Bar Chart**
  - Population by Gender

- **Donut Chart**
  - Marital Status Distribution

- **Pie Chart**
  - Ethnicity Distribution

- **Line Chart**
  - Births per Year

- **Table Visual**
  - First Name
  - Last Name
  - City
  - Gender

- **Slicer**
  - Race Filter

## Dashboard Preview

![Patient Dashboard](https://github.com/akisavujel/Power-BI/blob/6f162177fc44d19b9b89efc090a9ecc739a08c54/Patient-Data-Analysis/Patient-Dashboard.jpg)

## Tools Used

- Microsoft Power BI
- CSV Dataset
- Power Query
- DAX Measures

## Key Learnings

Through this project, I learned:

- Data cleaning and preprocessing in Power Query
- Creating calculated columns and measures
- Building interactive dashboard layouts
- Using different chart types for data storytelling
- Improving dashboard readability and usability

## Repository Structure

```bash
Patient-Data-Analysis/
│── Patient-Dashboard.jpg
│── Patient-Data-Analysis.pbix
│── README.md
```

## Author

**Akisha Bhujel**

- Portfolio: https://akishabhujel.github.io/myportfolio/
- GitHub: https://github.com/akisavujel
- LinkedIn: https://www.linkedin.com/in/akishabhujel/
