# 🏏 T20 World Cup Cricket Data Analytics: Finding the "Best 11"

## 🎯 Project Objective
The goal of this project is to build an end-to-end data analytics solution to assemble the ultimate "Best 11" T20 cricket team from the planet. Using data from the T20 World Cup, I extracted player performance metrics, processed the raw data, and built a dynamic Power BI dashboard to select players based on strict, data-driven parameters (e.g., batting average, strike rate, economy, and bowling strike rate).

## 🛠️ Tech Stack & Tools Used
* **Web Scraping:** JavaScript (BrightData)
* **Data Cleaning & Preprocessing:** Python, Pandas, JSON
* **Data Modeling & Visualization:** Power BI, DAX, Power Query
* **Presentation:** Microsoft PowerPoint (UI/UX Mockups)

## 📂 Project Structure & Pipeline
This repository contains the complete ETL (Extract, Transform, Load) pipeline, organized as follows:

* **`1_Data_Collection/`**: Contains the JavaScript code used to scrape real-time match and player data from ESPN Cricinfo.
* **`2_Raw_Data/`**: The scraped data stored in unstructured JSON format.
* **`3_Data_Preprocessing/`**: Contains the Python Jupyter Notebook (`.ipynb`) used to clean the JSON files, handle missing values, and flatten the data structures.
* **`4_Structured_Data/`**: The cleaned, transformed data exported as CSV files, ready for dimensional modeling (Fact and Dimension tables).
* **`5_Dashboard_and_Logic/`**: Contains the Power BI dashboard (`.pbix`), the DAX measures used for complex calculations, and the original parameter scoping document.

## 📊 Business Logic & Team Selection Criteria
The dashboard allows for dynamic filtering based on specific player roles. The criteria for the "Best 11" include:
1. **Openers (2):** Batting Avg > 30, Strike Rate > 140, Boundary % > 50.
2. **Anchors / Middle Order (3):** Batting Avg > 40, Strike Rate > 125, Avg Balls Faced > 20.
3. **Finisher / Lower Order Anchor (1):** Batting Avg > 25, Strike Rate > 130, Batting Position > 4.
4. **All-Rounders (2):** Batting Avg > 15, Strike Rate > 140, Bowling Economy < 7, Bowling Strike Rate < 20.
5. **Specialist Bowlers (3):** Bowling Economy < 7, Bowling Strike Rate < 16, Dot Ball % > 40.

## 📸 Final Dashboard
*(Note to self: Take a screenshot of your Power BI dashboard and drag-and-drop the image file right here in the GitHub editor to show off your work!)*

## 💡 Key Learnings
* Developed a complete ETL pipeline from scratch.
* Mastered complex DAX functions for custom sports analytics metrics.
* Designed a clean, user-friendly UI/UX for a BI dashboard based on standard design principles.
