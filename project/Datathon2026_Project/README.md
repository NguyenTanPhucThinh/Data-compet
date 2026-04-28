# Datathon 2026 - Giải pháp Dự báo Doanh thu (Team: [Tên Nhóm])

Giải pháp dự báo Revenue và COGS hàng ngày cho giai đoạn 2023 - 2024 sử dụng mô hình kết hợp (Ensemble) giữa Machine Learning và Statistical Modeling.

## 1. Cấu trúc thư mục
- `data/`: Chứa dữ liệu gốc (raw) và dữ liệu đã qua xử lý (processed).
- `notebooks/`:
    - `03_Part3_Data_Prep.ipynb`: Làm sạch và hợp nhất dữ liệu từ nhiều nguồn.
    - `04_Part3_Feature_Eng.ipynb`: Tạo các biến trễ (Lags), cửa sổ trượt (Rolling) và tích hợp Web Traffic.
    - `05_Part3_Modeling_SHAP.ipynb`: Huấn luyện mô hình Ensemble, dự báo đệ quy và giải thích bằng SHAP.
- `report/`: Chứa mã nguồn LaTeX và file báo cáo PDF theo định dạng NeurIPS.
- `submission/`: File `final_submission_ensemble.csv` nộp trên Kaggle.

## 2. Phương pháp tiếp cận
- **Mô hình:** Kết hợp **LightGBM** (tối ưu đặc trưng hành vi) và **Prophet** (tối ưu tính mùa vụ).
- **Chiến lược:** Dự báo đệ quy (Recursive Forecasting) từng ngày để cập nhật các biến trễ cho tương lai.
- **Giải thích:** Sử dụng **SHAP values** để phân tích mức độ ảnh hưởng của các chiến dịch Marketing và Web Traffic đến kết quả dự báo.

## 3. Hướng dẫn chạy lại kết quả (Reproducibility)
Để tái lập kết quả dự báo, vui lòng thực hiện theo các bước sau:

### Bước 1: Cài đặt môi trường
Cài đặt các thư viện cần thiết thông qua pip:
```bash
pip install -r requirements.txt