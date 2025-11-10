# Megaline Telecom Plan Analysis

This project analyzes the performance of Megaline's prepaid mobile plans **Surf** and **Ultimate** to determine which one generates higher revenue. The analysis provides insights to help the marketing team optimize advertising budget allocation.

This project demonstrates the ability to:
* Clean and prepare multi-table usage data for analysis.
* Calculate monthly revenue including overage charges.
* Compare user behavior and revenue performance across customer segments.

---

## The Challenge

The business goal was to identify which of the two mobile plans drives higher revenue and whether geography (NY-NJ vs. other regions) influences customer revenue.

Objectives:
1. Prepare and clean the datasets related to calls, internet, messages, plans, and users.
2. Aggregate user usage data and calculate total monthly revenue.
3. Perform exploratory analysis and hypothesis testing to compare revenue performance.

---

## My Solution & Key Files

### 1. Technical Analysis Notebook: `Analisis Telco.ipynb`
* Loaded and cleaned five datasets (calls, messages, internet, plans, users).
* Aggregated usage per customer per month and calculated overage fees.
* Calculated total revenue by combining base plan cost and additional usage charges.
* Conducted exploratory data analysis and visual comparisons of plan performance.
* Performed statistical hypothesis testing (t-tests) to compare mean revenue across plans and regions.

### 2. Data / Input Files
* `calls.csv`
* `internet.csv`
* `messages.csv`
* `plans.csv`
* `users.csv`

These datasets contain raw usage and customer plan information for the 2018 customer sample.

---

## Core Tools Used

* Python 3
* Pandas
* NumPy
* Matplotlib
* SciPy (stats)
