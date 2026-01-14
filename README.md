# Data_Mining_Customer_Churn_Prediction

💡 Tổng quan

Bài toán phân loại: xây dựng pipeline EDA → Tiền xử lý → Huấn luyện → Đánh giá → Submission với nhiều mô hình (Decision Tree, RandomForest, XGBoost/LightGBM/CatBoost).
Mục tiêu: tạo một khung làm việc tái sử dụng cho các bài toán tabular.

📦 Dữ liệu

Nguồn: (điền link hoặc mô tả dataset, ví dụ: “Kaggle – Titanic” hoặc “dataset nội bộ”)

Định dạng: train.csv, test.csv, cột mục tiêu (ví dụ Survived), cột phân loại/số.

🛠️ Phương pháp

Tiền xử lý: xử lý thiếu, mã hóa biến phân loại (One-Hot/Ordinal), chuẩn hóa/scale khi cần, chọn đặc trưng.

Mô hình: DecisionTree, RandomForest, XGBoost/LightGBM/CatBoost.

Đánh giá: Accuracy, Precision/Recall/F1, ROC-AUC; kèm ma trận nhầm lẫn & classification report.

CV: (Stratified) K-Fold để ước lượng ổn định.

<img width="1000" height="264" alt="image" src="https://github.com/user-attachments/assets/733b4664-3259-4e13-afa8-d91c8a8c4f5d" />
