 ## IPL Data Analysis (2008 - 2017)

A comprehensive Data Analysis project on Indian Premier League (IPL) matches dataset using **Python** and **Pandas**. This project explores match outcomes, team performances, toss impacts, venue insights, and team rivalries over a 10-year period.

---

##  Project Overview
The objective of this project is to perform Exploratory Data Analysis (EDA) on IPL historical data to unveil key patterns, strategic insights, and statistics about teams, players, and match outcomes.

---

##  Tech Stack & Methods Used
* **Language:** Python
* **Data Processing:** Pandas
* **Environment:** Jupyter Notebook / Google Colab
* **Key Pandas Techniques:** `groupby()`, `value_counts()`, `drop_duplicates()`, boolean indexing, dynamic filtering, data cleaning & imputation.

---

##  Data Cleaning & Preprocessing
* **Missing Value Imputation:** Filled missing values in the `city` column dynamically using corresponding venue locations.
* **Inplace Bug Fix for Missing Winners:** Correctly imputed missing values in the `winner` column using reassignment (`df['winner'] = df['winner'].fillna('No Result')`) to permanently persist changes in memory instead of temporary series outputs.
* **Team Name Standardization:** Standardized duplicate team name entries (e.g., merging `'Rising Pune Supergiant'` and `'Rising Pune Supergiants'` into a single normalized entity) using `.replace()` mapping to ensure precise win counts and team performance metrics.
* **Column Dropping:** Dropped the redundant `umpire3` column due to complete absence of historical records (100% null values).
---

##  Key Findings & Insights

### 1. Overall Match Stats
* **Total Matches Played:** 636
* **Most Successful Team:** Mumbai Indians (92 Wins), followed by Chennai Super Kings (79 Wins).
* **Most Player of the Match Awards:** CH Gayle (18 times), followed by YK Pathan (16 times).

### 2. Match Dynamics & Trends
* **Toss Impact:** The team winning the toss won the match **325 times** (~51.1%).
* **Toss Choice Preference:** Teams chose to **Field first (363 times)** significantly more than choosing to Bat first (273 times).
* **Chasing Advantage:** Teams bowling/chasing first won **53.30%** of total matches compared to 45.13% won by teams batting first.

### 3. Venue & Rivalry Highlights
* **Most Played Stadium:** M. Chinnaswamy Stadium (66 Matches).
* **Chinnaswamy Stadium Trend:** Chasing teams dominated with 36 wins compared to 27 wins for teams batting first.
* **(MI vs CSK Head-to-Head):** Mumbai Indians edge out Chennai Super Kings with a **12 - 10** head-to-head win record.
* **(RCB vs CSK Head-to-Head):** CSK won more matches rather than RCB **(6 - 4)**  win record.
### 4. Record Margin Victories
* **Largest Run Margin Victory:** Mumbai Indians defeated Delhi Daredevils by **146 runs** in 2017.
* **10-Wicket Victories:** Recorded 10 times in IPL history between 2008 and 2017.

---

##  Season Champions Summary
| Season | Champion |
| :---: | :--- |
| **2008** | Rajasthan Royals |
| **2009** | Deccan Chargers |
| **2010** | Chennai Super Kings |
| **2011** | Chennai Super Kings |
| **2012** | Kolkata Knight Riders |
| **2013** | Mumbai Indians |
| **2014** | Kolkata Knight Riders |
| **2015** | Mumbai Indians |
| **2016** | Sunrisers Hyderabad |
| **2017** | Mumbai Indians |

---

##  How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/pratapsingh23/ipl-data-analysis-pandas.git
