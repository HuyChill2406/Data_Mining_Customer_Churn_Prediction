# Bank Customer Churn Prediction 🏦📊 (English version below)

## 📖 Giới thiệu (Overview)
Dự án này tập trung vào việc xây dựng mô hình Machine Learning để dự đoán khả năng rời bỏ dịch vụ (Customer Churn) của khách hàng ngân hàng. Trong bối cảnh ngành tài chính cạnh tranh gay gắt, việc giữ chân khách hàng hiện tại quan trọng và tiết kiệm chi phí hơn nhiều so với việc tìm kiếm khách hàng mới.

Dự án không chỉ dừng lại ở việc huấn luyện mô hình mà còn đi sâu vào phân tích bối cảnh kinh doanh, xác định các yếu tố rủi ro và đề xuất các chiến lược giữ chân khách hàng dựa trên dữ liệu.

## 🎯 Mục tiêu Kinh doanh (Business Objectives)
Dựa trên phân tích bối cảnh thực tế:
- **Mục tiêu chính:** Giảm tỷ lệ khách hàng rời bỏ thông qua việc dự đoán sớm các khách hàng có nguy cơ cao.
- **Mục tiêu hỗ trợ:**
  - Xác định các yếu tố chính ảnh hưởng đến quyết định rời bỏ (ví dụ: phí dịch vụ, trải nghiệm khách hàng, đối thủ cạnh tranh).
  - Tối ưu hóa các chiến dịch giữ chân khách hàng (Retention Campaigns) bằng cách nhắm đúng đối tượng mục tiêu.
  - Cải thiện ROI cho các hoạt động Marketing và Chăm sóc khách hàng.

## 🗂️ Dữ liệu (The Data)
Bộ dữ liệu được sử dụng mô phỏng thông tin khách hàng ngân hàng (tương tự bộ dữ liệu Churn Modelling nổi tiếng), bao gồm 15,000 bản ghi với các đặc trưng:
- **Thông tin nhân khẩu học:** CustomerId, Surname, Geography, Gender, Age.
- **Thông tin tài chính:** CreditScore, Balance, EstimatedSalary.
- **Thông tin dịch vụ:** Tenure (thâm niên), NumOfProducts, HasCrCard, IsActiveMember.
- **Biến mục tiêu (Target):** `Exited` (1: Rời bỏ, 0: Ở lại).

*Nguồn dữ liệu: Kaggle Competitions.* : https://www.kaggle.com/competitions/bank-customer-churn-prediction-challenge/data

## 🛠️ Quy trình thực hiện (Workflow)
1. **Business Understanding:** Định nghĩa rõ vấn đề, mục tiêu và tiêu chí thành công (Success Criteria) từ góc độ kỹ thuật và kinh doanh.
2. **Data Understanding & EDA:**
   - Phân tích thống kê mô tả.
   - Kiểm tra dữ liệu thiếu (Missing values) và trùng lặp (Duplicates).
   - Phân tích đơn biến (Univariate Analysis) và phát hiện ngoại lai (Outlier Detection) sử dụng phương pháp IQR.
3. **Data Preprocessing:** Xử lý dữ liệu, làm sạch và chuẩn hóa.
4. **Modeling & Evaluation:** Xây dựng và đánh giá mô hình.

## 🚀 Công nghệ sử dụng (Tech Stack)
- **Ngôn ngữ:** Python
- **Thư viện:** Pandas, NumPy (Xử lý dữ liệu), Matplotlib, Seaborn (Trực quan hóa).
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
4. **Modeling & Evaluation:** Building and evaluating models (In Progress).

## 🚀 Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy (Data Processing), Matplotlib, Seaborn (Visualization).
- **Environment:** Jupyter Notebook / Google Colab.
