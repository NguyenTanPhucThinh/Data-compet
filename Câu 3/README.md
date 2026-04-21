•	Công cụ: xây dựng một pipeline hoàn chỉnh bao gồm các bước: Feature engineering, Cross-validation (phải đúng theo chiều thời gian), và các kỹ thuật xử lý rò rỉ dữ liệu (Leakage). Sử dụng hệ sinh thái Python (như Scikit-learn, XGBoost, hoặc LightGBM)
•	Nhiệm vụ: Dự báo cột Revenue cho giai đoạn 01/01/2023 – 01/07/2024.
•	Yêu cầu kỹ thuật:
o	Xây dựng Pipeline: Feature engineering, cross-validation đúng chiều thời gian và tuyệt đối không để rò rỉ dữ liệu (leakage) từ tập test.
o	Giải thích mô hình: Sử dụng SHAP values, Feature Importance hoặc Partial Dependence Plots để giải thích các yếu tố dẫn động doanh thu bằng ngôn ngữ kinh doanh.
Nộp bài: Upload file submission.csv lên hệ thống Kaggle theo đúng thứ tự dòng quy định.
•	Ràng buộc:
o	Không dùng dữ liệu ngoài
o	Tính tái lập: Đính kèm toàn bộ mã nguồn, đặt random seed
o	Khả năng giải thích: Trong report, bao gồm một mục giải thích các yếu tố dẫn động doanh thu chính được mô hình xác định (vd: feature importances, SHAP values hoặc partial dependence plots). Giải thích mô hình học được gì bằng ngôn ngữ kinh doanh
•	Chỉ số đánh giá: MAE và RMSE càng thấp càng tốt. R^2  càng cao càng tốt (lý tưởng gần 1).
LINK DATASET: https://www.kaggle.com/competitions/datathon-2026-round-1/overview
NỘP KẾT QUẢ TRÊN LINK KAGGLE NÀY:  https://www.kaggle.com/competitions/datathon-2026-round-1
