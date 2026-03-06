Here is your complete **Markdown Assignment File** ready to give to students 👇

You can copy this into a `.md` file (Example: `Loan_Prediction_Dashboard_Assignment.md`)

---

# 📘 Assignment: Loan Prediction System Dashboard

---

## 🎯 Objective

Design and develop a **Loan Prediction System Dashboard** by converting a Machine Learning model into:

* A REST API (Backend Layer)
* An Interactive Dashboard (Frontend Layer)

The dashboard must visualize model performance, dataset insights, and allow real-time loan prediction.

---

# 🧠 Given Machine Learning Model

The following ML pipeline has already been implemented:

### ✔ Steps Performed in Model

1. Data loading (`loan_data.csv`)
2. Dropping unnecessary column (`Loan_ID`)
3. Handling missing values
4. Encoding categorical variables
5. Feature scaling
6. Train-test split (80-20)
7. Model training using `RandomForestClassifier`
8. Evaluation using:

   * Accuracy
   * Confusion Matrix
   * Classification Report

### ✔ Model Performance

```
Accuracy: 0.7878

Confusion Matrix:
[[18 16]
 [ 5 60]]

Classification Report:

Class 0:
Precision: 0.78
Recall: 0.53
F1-score: 0.63

Class 1:
Precision: 0.79
Recall: 0.92
F1-score: 0.85
```

---

# 🏗️ PART 1 – Backend Development (API Layer)

Convert the ML script into a REST API.

## 📌 Required API Endpoints

### 1️⃣ System Endpoints

* `GET /api/health`
* `GET /api/model/info`

### 2️⃣ Model Performance

* `GET /api/model/metrics`
* `GET /api/model/confusion-matrix`
* `GET /api/model/classification-report`

### 3️⃣ Feature Analysis

* `GET /api/model/feature-importance`

### 4️⃣ Dataset Insights

* `GET /api/data/loan-distribution`
* `GET /api/data/property-area-analysis`
* `GET /api/data/income-loan-scatter`
* `GET /api/data/credit-history-impact`

### 5️⃣ Prediction Endpoint

* `POST /api/predict`

### 6️⃣ Prediction History

* `GET /api/predictions/recent`
* `DELETE /api/predictions/clear`

### 7️⃣ Optimized Dashboard Endpoint

* `GET /api/dashboard/summary`

---

## 🔧 Backend Requirements

* Use Flask (or FastAPI)
* Return structured JSON responses
* Perform preprocessing inside prediction endpoint
* Store recent predictions (in-memory or file-based)
* Ensure proper error handling
* Use REST conventions

---

# 🎨 PART 2 – Frontend Dashboard Development

Develop a responsive dashboard using:

* Bootstrap 5
* Chart.js / DC.js
* Fetch API (to connect backend)

---

# 📊 Dashboard Layout Structure

```
----------------------------------------------------------
| Loan Prediction System Dashboard                      |
----------------------------------------------------------
| KPI Cards                                             |
----------------------------------------------------------
| Confusion Matrix  | Classification Metrics Chart      |
----------------------------------------------------------
| Feature Importance Chart                              |
----------------------------------------------------------
| Loan Distribution | Property Area Analysis            |
----------------------------------------------------------
| Income vs Loan Amount Scatter Plot                    |
----------------------------------------------------------
| Loan Prediction Form                                  |
----------------------------------------------------------
| Recent Predictions Table                              |
----------------------------------------------------------
```

---

# 🧩 Dashboard Sections (Detailed Requirements)

---

## 1️⃣ Header Section

* Title
* Model name
* Accuracy display
* Last updated timestamp

---

## 2️⃣ KPI Cards

Display:

* Model Accuracy
* Total Test Samples
* Approved Loans Count
* Rejected Loans Count

---

## 3️⃣ Confusion Matrix

* 2×2 Heatmap
* Display TP, TN, FP, FN
* Add short interpretation text

---

## 4️⃣ Classification Metrics Chart

Bar chart showing:

* Precision (Class 0 & 1)
* Recall (Class 0 & 1)
* F1-score (Class 0 & 1)

---

## 5️⃣ Feature Importance Chart

* Horizontal bar chart
* Sorted descending
* Tooltip with feature importance value

---

## 6️⃣ Loan Distribution

* Pie or Donut chart
* Approved vs Rejected percentage

---

## 7️⃣ Property Area Analysis

* Grouped Bar Chart
* Urban vs Rural vs Semiurban
* Approved vs Rejected

---

## 8️⃣ Income vs Loan Amount

* Scatter plot
* Color based on Loan_Status

---

## 9️⃣ Live Loan Prediction Form

### Required Fields:

* Gender
* Married
* Dependents
* Education
* Self Employed
* Applicant Income
* Coapplicant Income
* Loan Amount
* Loan Term
* Credit History
* Property Area

### Output Display:

* Prediction (Approved/Rejected)
* Probability Score
* Confidence Indicator

---

## 🔟 Recent Predictions Table

Display:

* Applicant Income
* Loan Amount
* Credit History
* Property Area
* Prediction
* Probability
* Timestamp

---

# 📱 Responsiveness Requirements

| Device  | Layout               |
| ------- | -------------------- |
| Desktop | Two-column grid      |
| Tablet  | Stacked charts       |
| Mobile  | Single column layout |

---

# 🎯 Expected Learning Outcomes

Students will learn:

* Converting ML model into REST API
* Model evaluation visualization
* Connecting frontend with backend
* Real-time prediction handling
* Dashboard design principles
* Data storytelling with charts

---

# 📦 Deliverables

Students must submit:

1. Backend Source Code
2. Frontend Source Code
3. README file
4. Screenshots of dashboard
5. API documentation
6. Short explanation document (2–3 pages)

---

# ⭐ Bonus Features (Optional)

* ROC Curve visualization
* Dark Mode toggle
* Export prediction report (CSV/PDF)
* Model retraining endpoint
* Threshold adjustment slider

---

# 🏆 Evaluation Criteria

| Criteria                     | Marks |
| ---------------------------- | ----- |
| Backend API Implementation   | 20    |
| Frontend Design              | 20    |
| Data Visualization           | 20    |
| API Integration              | 20    |
| Code Quality & Documentation | 10    |
| Innovation / Extra Features  | 10    |

---

# ⏳ Submission Deadline

(To be filled by Instructor)

---

# 👨‍🏫 Instructor Notes

Students should focus on:

* Clean UI design
* Meaningful data visualization
* Proper API structure
* Error handling
* Professional presentation

---

If you would like, I can next provide:

* ✅ A ready-made student grading rubric (detailed)
* ✅ A mini project report template (IEEE style)
* ✅ A frontend folder structure template
* ✅ A backend architecture diagram
* ✅ A ready-to-use README template

Let me know 👍
