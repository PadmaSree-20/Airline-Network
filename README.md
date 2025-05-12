# ✈️ The Role of Network Design in Airline Performance — A Data-Driven Study

This project investigates how airline network structures (Hub-and-Spoke vs. Point-to-Point) influence operational efficiency and on-time performance. Using statistical modeling, machine learning, and network analysis, it evaluates U.S. legacy and low-cost carriers, offering insights into route strategy and optimization.

---

## 📘 Abstract

Airlines operate in a complex environment where network design significantly affects delays, capacity utilization, and passenger satisfaction. This project compares the **Hub-and-Spoke** and **Point-to-Point** systems through a data-driven lens, analyzing metrics such as **arrival delays**, **load factors**, **stage lengths**, and **network centrality**.

---

## 📊 Data Sources

- **Bureau of Transportation Statistics**
  - On-Time Performance Data (2018)
  - T-100 Segment Traffic Data (2018–2023)

### Key Metrics Derived:
- Arrival Delay, Departure Delay
- Load Factor = RPM / ASM
- Stage Length = Distance / Departures
- Block Time Efficiency = Air Time / Ramp Time
- Congestion at Origin
- Flight Time Efficiency

---

## 🧪 Models Used

### 📈 Linear Regression
- Implemented using both `statsmodels` and `sklearn`
- Feature selection via p-value significance and forward selection
- Adjusted R² ≈ 0.96 with statistically significant predictors

### 🌳 Decision Tree Regressor
- Developed with `sklearn.tree.DecisionTreeRegressor`
- Tuned using `max_depth` (best at depth 13)
- R² up to 0.98 (high generalization accuracy)

---

## 🌐 Network Analysis

Using the `networkx` library, the airline networks are visualized and analyzed by centrality metrics:
- **Degree Centrality** – direct connectivity
- **Betweenness Centrality** – role in connecting paths
- **Closeness Centrality** – average distance to other nodes
- **Eigenvector Centrality** – influence based on connected hubs

### 🛫 Carriers Analyzed:
- American Airlines
- Delta Air Lines
- United Airlines
- Southwest Airlines

> Legacy carriers show centralized (hub-based) structures; Southwest's network is more distributed, reflecting a Point-to-Point model.

---

## 🗂️ Repository Structure

```bash
├── Network Analytics.ipynb     # Full notebook with model development and analysis
├── Final Report.pdf            # Detailed report with literature, methods, and results
├── README.md                   # Project overview (this file)

```

## 📎 Academic Acknowledgment (Original Submission)
This work was originally submitted as part of:

- Course: DSCI 5900 — Special Problems
- Institution: University of North Texas
- Instructor: Dr. Sourav Chatterjee
- Author: Padma Sree Manda
- Date: Dec 2024
Special thanks to Harley Moulder for guidance on the airline industry throughout the research process.

---

## 🧑‍💻 Maintainer

- **Padma Sree Manda**
- Feel free to reach out via LinkedIn or padma20manda@gmail.com

---

## 📄 License

This project is shared for educational and demonstration purposes.