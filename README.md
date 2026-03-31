# AI--powered-Loan-Approval-prediction-in-logistic-regression.
🏦 AI-Powered Loan Approval Prediction Dashboard

A production-style Machine Learning project that predicts whether a customer’s loan request will be approved or rejected using Logistic Regression.
This project combines data preprocessing, feature engineering, predictive analytics, and an interactive 3D dashboard to simulate a real banking decision-support system.

It is designed as a mini project / final-year ML project / GitHub portfolio project with a modern analytics workflow.


🌟 project Objective

The main goal is to help banks and fintech systems reduce manual verification time by automatically estimating the probability of loan approval.
The system analyzes customer financial details such as:
income
co-applicant income
requested loan amount
repayment term
credit history
property area
and predicts the final decision.

🚀 Key Features

✅ Binary classification using Logistic Regression
📂 Supports CSV dataset input
🧹 Data cleaning + missing value handling
⚙️ Feature engineering for risk analysis
📊 KPI-based dashboard metrics
🌌 Interactive moveable Plotly 3D visualization
🔍 Real-time applicant prediction
📈 Approval vs rejection analytics
🌐 Streamlit web dashboard
☁️ Ready for cloud deployment
 
📂 Dataset Description

🎯 Input Features
ApplicantIncome
CopplicantIncome
LoanAmount
Loan_Amount_Term
Credit_History
Property_Area

🎯 Target Variable
Loan_Status
1 → Approved ✅
0 → Rejected ❌

✨ Feature Engineering

To improve business insights, extra features are created:
df["TotalIncome"] = df["ApplicantIncome"] + df["CoapplicantIncome"]
df["EMI"] = df["LoanAmount"] / df["Loan_Amount_Term"]
df["RiskScore"] = df["LoanAmount"] / df["TotalIncome"]

📌 Why these matter
TotalIncome → applicant repayment strength
EMI → monthly repayment burden
RiskScore → loan-to-income ration
These features make the dashboard more realistic.

🧠 Machine Learning Pipelie

1. 📥 Read dataset from CSV
2. 🧹 Handle missing values
3. 🏗️ Create engineered features
4. 🔄 Scale data using StandardScaler
5. ✂️ Split into train/test
6. 🤖 Train Logistic Regression model
7. 📈 Evaluate accuracy
8. 🌐 Deploy in Streamlit dashboard

📊 Dashboard Analytics

The Streamlit dashboard contains:

📌 KPI Cards

Total Applications
Total Approved
Total Rejected
Approval Rate
Average Loan Amount
High Risk Applicants


📌 Visual Analytics

📈 Approval vs Rejection bar chart
💰 Income distribution histogram
📉 Loan amount vs approval scatter plot

🌌 3D moveable Plotly scatter dashboard

🌌 Interactive 3D Visualization
A realistic Plotly 3D scatter plot is used for advanced analytics.

📍 Graph Axes

X-axis → Applicant Income
Y-axis → Loan Amount
Z-axis → Credit History
Bubble Size → Total Income
Bubble Color → Loan Status


🎯 Benefits

This helps banking teams visually identify:
low-risk applicants
high-risk clusters
approval regions
rejection patterns
customer income segments
The graph is fully rotatable, zoomable, and moveable.

🛠️ Tech Stack
Python
Pandas
NumPy
Scikit-learn
Plotly
Streamlit
Google Colab / Jupyter

▶️ Installation & Run

pip install pandas numpy scikit-learn plotly streamlit
streamlit run app.py

📁 Recommended GitHub Structure

loan-approval-dashboard/
│── app.py
│── loan_data.csv
│── requirements.txt
│── README.md
│── assets/
│   └── dashboard_screenshot.png


📊 Expected Results

🎯 Accuracy: 85–92%
🏦 Real-time approval prediction
🌌 Interactive 3D dashboard
📈 Risk analytics
💼 Banking-style UI

💼 Real-World Applications

This project can be used in:
digital banking systems
NBFC loan approval
BNPL apps
credit risk scoring
EMI eligibility systems
fintech underwriting tools

🔮 Future Enhancements
🌲 Random Forest / XGBoost comparison
🤖 probability score output
📱 mobile responsive dashboard
🔐 admin login system
📄 downloadable PDF reports
☁️ deployment on Streamlit Cloud
🔔 applicant alert notifications

👨‍💻 Author
Jashwanth sariputi
Machine Learning | Data Science | Dashboard Projects 🚀
