# YÊU CẦU MÔ HÌNH DỰ BÁO REVENUE

## Công cụ

Xây dựng một **pipeline hoàn chỉnh** sử dụng hệ sinh thái Python, có thể dùng:

- Scikit-learn  
- XGBoost  
- LightGBM  

Pipeline cần bao gồm:

- Feature Engineering  
- Cross-validation đúng theo chiều thời gian  
- Các kỹ thuật xử lý rò rỉ dữ liệu (Data Leakage Prevention)  

---

## Nhiệm vụ

Dự báo cột **Revenue** cho giai đoạn:

**01/01/2023 – 01/07/2024**

---

## Yêu cầu kỹ thuật

### 1. Xây dựng Pipeline

Pipeline phải đảm bảo:

- Có bước feature engineering rõ ràng  
- Cross-validation đúng theo thứ tự thời gian (Time Series Split)  
- Tuyệt đối không để rò rỉ dữ liệu từ tập test sang train  

### 2. Giải thích mô hình

Sử dụng ít nhất một trong các phương pháp sau:

- SHAP Values  
- Feature Importance  
- Partial Dependence Plots  

Mục tiêu:

- Giải thích các yếu tố ảnh hưởng đến doanh thu  
- Trình bày bằng ngôn ngữ kinh doanh dễ hiểu  

---

## Nộp bài

- Tạo file **submission.csv**  
- Upload lên hệ thống Kaggle theo đúng thứ tự dòng quy định  

### Link Dataset

https://www.kaggle.com/competitions/datathon-2026-round-1/overview

### Link Nộp Bài

https://www.kaggle.com/competitions/datathon-2026-round-1

---

## Ràng buộc

### Không sử dụng dữ liệu ngoài

- Chỉ được phép dùng dữ liệu do cuộc thi cung cấp  

### Tính tái lập

- Đính kèm toàn bộ mã nguồn  
- Đặt random seed cố định  

### Khả năng giải thích

Trong report cần có một mục riêng *** SỬ DỤNG LATEX *** để giải thích:

- Những yếu tố dẫn động doanh thu chính do mô hình xác định  
- Có thể dùng:
  - Feature Importance  
  - SHAP Values  
  - Partial Dependence Plot  

Giải thích mô hình học được gì bằng ngôn ngữ kinh doanh.

---

## Chỉ số đánh giá

Mô hình càng tốt khi:

- **MAE** càng thấp càng tốt  
- **RMSE** càng thấp càng tốt  
- **R²** càng cao càng tốt (lý tưởng gần **1**)

***LƯU Ý: CẦN CHỨA MÃ NGUỒN, NOTEBOOK VÀ SUBMISSION***
