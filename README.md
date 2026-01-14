# 🏦📊 Bank Customer Churn Prediction (English version below)

## 🇻🇳 Giới thiệu (Overview)
Dự án này tập trung xây dựng pipeline Machine Learning hoàn chỉnh nhằm dự đoán khả năng khách hàng ngân hàng rời bỏ dịch vụ (Customer Churn).
Trong bối cảnh ngành tài chính cạnh tranh cao, việc xác định sớm các khách hàng có nguy cơ rời bỏ giúp ngân hàng triển khai các chiến lược giữ chân hiệu quả và tiết kiệm chi phí hơn so với việc thu hút khách hàng mới.

Bên cạnh huấn luyện mô hình, dự án nhấn mạnh Business Understanding, phân tích nguyên nhân rời bỏ và đánh giá tác động của các quyết định kỹ thuật đến hiệu quả kinh doanh.

## 🎯 Mục tiêu Kinh doanh (Business Objectives)
Dựa trên phân tích bối cảnh thực tế:
- **Mục tiêu chính:** Giảm tỷ lệ khách hàng rời bỏ thông qua việc dự đoán sớm các khách hàng có nguy cơ cao.
- **Mục tiêu hỗ trợ:**
  - Xác định các yếu tố chính ảnh hưởng đến quyết định rời bỏ (ví dụ: phí dịch vụ, trải nghiệm khách hàng, đối thủ cạnh tranh).
  - Tối ưu hóa các chiến dịch giữ chân khách hàng (Retention Campaigns) bằng cách nhắm đúng đối tượng mục tiêu.
  - Cải thiện ROI cho các hoạt động Marketing và Chăm sóc khách hàng.

## 🗂️ Dữ liệu (The Data)
**Nguồn**: Kaggle – Bank Customer Churn Prediction Challenge (https://www.kaggle.com/competitions/bank-customer-churn-prediction-challenge/data).
**Quy mô**: ~15,000 bản ghi
**Biến đầu vào**:
- **Thông tin nhân khẩu học:** CustomerId, Surname, Geography, Gender, Age.
- **Thông tin tài chính:** CreditScore, Balance, EstimatedSalary.
- **Thông tin dịch vụ:** Tenure (thâm niên), NumOfProducts, HasCrCard, IsActiveMember.
**Biến mục tiêu (Target):** `Exited` (1: Rời bỏ, 0: Ở lại).

## 🛠️ Quy trình thực hiện (Workflow)
1️⃣ Business Understanding

- Định nghĩa bài toán churn prediction từ góc độ kinh doanh và kỹ thuật.

- Xác định tiêu chí thành công, tập trung vào khách hàng rời bỏ (class 1).

2️⃣ Data Understanding & EDA

- Thống kê mô tả cho biến số và biến phân loại.

- Kiểm tra dữ liệu thiếu và trùng lặp.

- Phân tích đơn biến và phát hiện ngoại lai bằng IQR method.

- Phân tích mối quan hệ giữa các đặc trưng và churn.

3️⃣ Data Preprocessing & Feature Engineering

- Thử nghiệm nhiều chiến lược tiền xử lý: One-hot encoding (Dummies), Label encoding (Catcode), Feature binning + encoding

- Xử lý class imbalance bằng undersampling (giảm lớp đa số).

- So sánh hiệu quả với các phương pháp scaling: StandardScaler, MinMaxScaler

4️⃣ Modeling & Evaluation

- Huấn luyện và benchmark nhiều mô hình: Logistic Regression, Decision Tree, Random Forest, Extra Trees, XGBoost, LightGBM, CatBoost

- Đánh giá bằng Stratified K-Fold Cross Validation (k = 5).

- Tập trung vào các metric quan trọng cho churn: Precision / Recall / F1-score (class 1), ROC-AUC

5️⃣ Model Selection & Persistence

- Lựa chọn mô hình tốt nhất dựa trên F1-score của churn class.

- Lưu model và scaler bằng joblib để tái sử dụng.

- Phân tích feature importance cho các mô hình cây.

6️⃣ Deployment-oriented Output

- Sinh file Kaggle submission từ model đã lưu.

- Xuất bảng benchmark chi tiết ra Excel để so sánh mô hình.

## 🚀 Công nghệ sử dụng (Tech Stack)
- **Ngôn ngữ:** Python
- **Thư viện:** Pandas, NumPy (Xử lý dữ liệu), Matplotlib, Seaborn (Trực quan hóa), Scikit-learn, XGBoost, LightGBM, CatBoost
- **Môi trường:** Jupyter Notebook / Google Colab.

-------------------------------------------------------------

# Bank Customer Churn Prediction 🏦📊

## 📖 Overview
This project focuses on building a Machine Learning model to predict bank customer churn. In the fiercely competitive financial landscape, retaining existing customers is crucial and far more cost-effective than acquiring new ones.

Beyond model training, this project dives deep into **Business Understanding**, analyzing the business context to identify risk factors and proposing data-driven retention strategies.

## 🎯 Business Objectives
Based on the real-world business context analysis:
- **Primary Objective:** Reduce customer churn rate by early identification of high-risk customers.
- **Supporting Objectives:**
  - Identify key factors influencing churn decisions (e.g., service fees, customer experience, competitor offers).
  - Optimize Retention Campaigns by targeting the right audience.
  - Improve ROI for Marketing and Customer Service activities.

## 🗂️ The Data
The dataset simulates bank customer information (similar to the famous Churn Modelling dataset), consisting of 15,000 records with features such as:
- **Demographics:** CustomerId, Surname, Geography, Gender, Age.
- **Financial Status:** CreditScore, Balance, EstimatedSalary.
- **Services:** Tenure, NumOfProducts, HasCrCard, IsActiveMember.
- **Target Variable:** `Exited` (1: Churn, 0: Retain).

*Data Source: Kaggle Competitions.* : https://www.kaggle.com/competitions/bank-customer-churn-prediction-challenge/data

## 🛠️ Workflow
1. **Business Understanding:** Clearly define the problem, objectives, and Success Criteria from both technical and business perspectives.
2. **Data Understanding & EDA:**
   - Descriptive statistics.
   - Checking for Missing values and Duplicates.
   - Univariate Analysis and Outlier Detection using the IQR method.
3. **Data Preprocessing:** Data cleaning, normalization, and feature engineering.
4. **Modeling & Evaluation:** Building and evaluating models (Logistic Regression, Decision Tree, Random Forest, Extra Trees, XGBoost, LightGBM, CatBoost).

## 🚀 Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy (Data Processing), Matplotlib, Seaborn (Visualization).
- **Environment:** Jupyter Notebook / Google Colab.
