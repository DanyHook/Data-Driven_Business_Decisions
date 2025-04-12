# Data-Driven_Business_Decisions
# 📦 Sprint 10 – Final Project: Data-Driven Business Decision Making

Congratulations! You’ve completed the "Data-Driven Business Decisions" course. Now it's time to apply what you've learned in a real-world analytical case study. This final project involves prioritizing business hypotheses and conducting an A/B test to support decision-making.

---

## 📚 Project Description

### 🔎 Context

You are working as a data analyst at a large online store. Together with the marketing team, you've gathered a list of hypotheses that may help increase revenue. Your task is to **prioritize these hypotheses**, **run an A/B test**, and **analyze the results** to guide the business on which strategy to adopt.

---

## 📁 Datasets

### Part 1 – Hypothesis Prioritization

**File:** `/datasets/hypotheses_us.csv`

| Column      | Description                                              |
|-------------|----------------------------------------------------------|
| Hypothesis  | Brief description of the idea                            |
| Reach       | Estimated reach on a scale from 1 to 10                  |
| Impact      | Estimated impact on users (scale from 1 to 10)           |
| Confidence  | Confidence in the hypothesis (scale from 1 to 10)        |
| Effort      | Resources required to test the hypothesis (scale 1–10)   |

### Part 2 – A/B Test Data

**Files:**  
- `/datasets/orders_us.csv`  
- `/datasets/visits_us.csv`

**orders_us.csv**

| Column         | Description                                      |
|----------------|--------------------------------------------------|
| transactionId  | Unique order ID                                  |
| visitorId      | Unique visitor ID                                |
| date           | Date of the order                                |
| revenue        | Revenue from the order                           |
| group          | A/B test group (A or B)                          |

**visits_us.csv**

| Column | Description                                               |
|--------|-----------------------------------------------------------|
| date   | Date of the visit                                         |
| group  | A/B test group (A or B)                                   |
| visits | Number of visits on that date within the specified group |

**Note:** Ensure proper data preprocessing. Some visitors may have appeared in both groups, which could affect the integrity of your test.

---

## 🚀 Part 1 – Hypothesis Prioritization

In this phase, you will:

- Apply the **ICE framework** to prioritize hypotheses by impact, confidence, and effort.
- Apply the **RICE framework**, which also accounts for reach.
- Compare both rankings and explain how reach affects prioritization.

---

## 📊 Part 2 – A/B Test Analysis

You conducted an A/B test and will analyze the outcomes using the `orders` and `visits` data.

### Your tasks:

1. **Cumulative Revenue**  
   - Plot cumulative revenue by group  
   - Draw conclusions and insights

2. **Average Order Value**  
   - Plot cumulative average order size by group  
   - Analyze trends and spikes

3. **Relative Difference**  
   - Plot relative difference in order value between Group B and Group A

4. **Daily Conversion Rate**  
   - Calculate conversion rate = orders / visits  
   - Visualize and compare daily conversion trends across groups

5. **Order Count per User**  
   - Scatter plot of orders per user  
   - Identify patterns and possible outliers

6. **Outlier Detection – Order Count**  
   - Calculate 95th and 99th percentiles for order frequency  
   - Define anomaly thresholds

7. **Outlier Detection – Order Price**  
   - Scatter plot of order prices  
   - Calculate 95th and 99th percentiles for revenue  
   - Define anomaly thresholds

8. **Statistical Testing (Raw Data)**  
   - Z-test for difference in conversion rates  
   - T-test for difference in average order size

9. **Statistical Testing (Filtered Data)**  
   - Repeat Z-test and T-test after removing outliers  
   - Assess the robustness of the results

10. **Final Decision Making**  
    - Based on statistical results, decide:  
      1. Stop the test and select a winner  
      2. Stop the test with no significant difference  
      3. Continue the test for more data

---

## ✅ Final Deliverables

- Jupyter Notebook with all analysis steps, graphs, and interpretations
- Business recommendations supported by statistical evidence
- Markdown cells explaining your logic and conclusions

---

## 🏁 Evaluation Criteria

Your project will be reviewed based on:

- Data cleaning and preprocessing
- Correct application of prioritization frameworks
- Quality and clarity of visualizations
- Soundness of statistical methods
- Interpretation of results
- Final decision and justification
- Clear communication in code and markdown

---

## 📌 Good luck and happy analyzing!
