# Yandex-Afisha-Ticket-Orders-Analysis

Focus areas:
- exploratory data analysis
- data visualization
- statistical hypothesis testing
- user behavior analysis


📖 Project Description

This project analyzes ticket order data from Yandex Afisha, an online event ticket platform.The analysis focuses on user behavior, ticket sales, revenue trends, and event popularity.The dataset covers the period June – October 2024. The project includes data preprocessing, exploratory data analysis (EDA), visualization, and hypothesis testing.The goal is to find useful insights about customer behavior and ticket demand.

🎯 Objectives

The main objectives of this project are:

1. Understand how users buy tickets
2. Analyze order trends over time
3. Identify popular events and partners
4. Study seasonal changes in demand
5. Analyze ticket prices and revenue
6. Test statistical hypotheses about user behavior

📊 Project Workflow

The analysis follows these main steps:

1️⃣ Data Understanding
Study dataset structure and column meanings.

2️⃣ Data Cleaning
Check missing values
Detect duplicates
Convert data types
Optimize memory usage

3️⃣ Feature Engineering
Create new variables for better analysis.

4️⃣ Exploratory Data Analysis (EDA)
Order trends over time
User activity
Revenue distribution
Popular events and partners

5️⃣ Statistical Analysis
Test hypotheses about differences in user behavior.

📂 Datasets

The project uses three datasets.

1️⃣ Orders Dataset
final_tickets_orders_df.csv

Contains information about ticket orders.

Important columns:

order_id — unique order ID
user_id — user identifier
created_dt_msk — order date
created_ts_msk — order timestamp
event_id — event identifier
tickets_count — number of tickets in the order
device_type — device type (mobile / desktop)
revenue_kzt — revenue in KZT

Dataset size:
290,849 rows
14 columns

2️⃣ Events Dataset
final_tickets_events_df.csv

Contains information about events.

Important columns:
event_id
city_id
venue_id
event categories
event location

Dataset size:
22,427 rows
11 columns

3️⃣ Currency Dataset

final_tickets_tenge_df.csv

Contains exchange rate information.

This dataset is used to convert revenue from KZT to RUB.

Dataset size:
357 rows
4 columns

⚙️ Technologies Used

This project uses the following tools:
Python
Pandas
Matplotlib
Seaborn
SciPy

🧹 Data Preprocessing

The following preprocessing steps were performed:

Checked dataset structure

Converted columns to correct data types

Optimized memory usage

Checked missing values

Removed duplicates

Created new analytical features

New Features Created

revenue_rub
Revenue converted from KZT to RUB using exchange rates.

one_ticket_revenue_rub
Average revenue per ticket.

📊 Exploratory Data Analysis
📅 Order Trends and Seasonality

Order activity was analyzed over time.

Key observations:

Ticket demand increases in autumn

Some event types become more popular

Average ticket price decreases in some categories

Possible reasons:

seasonal promotions

audience preferences

growth of large entertainment events

👥 User Activity

User behavior was analyzed using:

total number of orders

number of unique users

Key insights:

Both orders and users increase over time

Orders grow faster than the number of users

Users may buy tickets more frequently

🎭 Popular Events and Partners

The analysis identifies:

partners with the highest revenue

partners with the most events

most popular event categories

regions with the highest demand

Important insight:

A small number of partners generate a large share of revenue.

💰 Revenue Analysis

Revenue distributions were analyzed.

Main observations:

Revenue values have high variability

Some outliers exist

Most orders have moderate revenue

Because the dataset is large, extreme values do not strongly affect the results.

📉 Statistical Hypothesis Testing

A statistical test was performed to compare mobile and desktop users.

Research Question

Do mobile users make more orders than desktop users?

Hypotheses

H0 (Null Hypothesis)
The average number of orders per user is the same for mobile and desktop users.

H1 (Alternative Hypothesis)
Mobile users make more orders on average.

Method Used

The analysis uses Welch’s t-test, which is appropriate when variances are different.

🔎 Key Insights

Main findings of the project:

Ticket demand increases during autumn

User activity grows over time

Mobile and desktop users behave differently

Some partners generate most of the revenue

Event popularity changes depending on season
