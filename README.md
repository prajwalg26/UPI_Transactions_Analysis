# UPI Transactions Analysis

## Project Overview
This project analyzes **2.5 lakh+ UPI transaction records** to explore:
- **Transaction categories & demographics**
- **Usage patterns by time, state, and merchant type**
- **Seasonal & hourly behavior**
- **Fraud pattern detection** using category and time-slot analysis

The insights can help **banks, fintech firms, and regulators** improve digital payment strategies, monitor anomalies, and enhance fraud detection mechanisms.

---

## Objectives
- Identify **distribution** of P2P (Person-to-Person) vs P2M (Person-to-Merchant) transactions.
- Pinpoint **top contributing states** and their share in total volume.
- Analyze **seasonality, hourly patterns, and peak usage times**.
- Detect **high-risk merchant categories and time slots** prone to fraudulent activity.
- Create **interactive Tableau dashboards** for data storytelling.


---

## Project Workflow

### 1️⃣ Data Cleaning & Preparation (Python — Pandas, NumPy)
- Removed duplicate transaction IDs.
- Handled null/missing values for `State` and `Merchant_Category`.
- Standardized categorical values (e.g., merchant category naming).
- Extracted new features:
  - **Hour**, **Month**, **Day of Week** from transaction timestamps.
  - **Season** mapping for seasonal analysis.

### 2️⃣ Exploratory Data Analysis
Key analyses performed:
- **P2P vs P2M share** in volume & value terms.
- **State-wise rankings** & top 5 states’ contribution (~40% transactions).
- **Age and gender-based preferences** in P2P/P2M usage.
- Seasonality trends (e.g., festive spikes).
- Hourly distribution for identifying **peak usage windows**.

### 3️⃣ Fraud Pattern Detection
- Grouped transactions by **Merchant_Category** & **Hour** to detect unusual spikes.
- Analyzed fraud flag distribution across categories/time slots.
- Flagged **high-risk combinations** for targeted monitoring.

### 4️⃣ Data Visualization (Tableau)
Developed interactive dashboards:
1. **Transaction Overview Dashboard** — P2P/P2M trends, volumes, and amounts.
2. **State & Demographics Dashboard** — State heatmap, age-gender breakdown.
3. **Fraud Risk Dashboard** — High-risk time slots & merchant profiles.

---

## Key Insights
- **P2P & P2M** dominate transaction volume (>90% combined).
- **Top 5 states** contribute ~40% of transactions.
- Evening hours (6 PM–9 PM) show **peak activity**.
- Festive months (Oct-Dec) have significant transaction spikes.
- Fraud risk concentrated in specific merchant categories during late-night hours.

---

## Tools & Technologies
| Tool / Library   | Purpose |
|------------------|---------|
| **Python**       | Data preprocessing, analysis |
| **Pandas, NumPy**| Cleaning, transformation, feature engineering |
| **Tableau**      | Interactive dashboard creation |
| **Matplotlib**   | Basic visual validation |
| **Seaborn**      | Statistical data visualization |
| **Jupyter Notebook** | Step-by-step analysis |

---

## Dashboard Preview
<img width="595" height="475" alt="download" src="https://github.com/user-attachments/assets/4c5fd983-252b-422f-9aa0-0414f58e6345" />
<img width="729" height="405" alt="download" src="https://github.com/user-attachments/assets/da668326-6876-4680-8278-24cedb548d54" />

---

