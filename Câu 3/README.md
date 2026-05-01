# Datathon 2026 - Part 3: Forecasting & SHAP

Phần này trình bày pipeline dự báo **Revenue** và **COGS** theo ngày cho giai đoạn 2023 - 2024, kết hợp giữa machine learning, feature engineering và giải thích mô hình bằng SHAP.

## Mục tiêu

Tôi đang xây dựng một quy trình dự báo có thể tái lập gồm 3 bước chính:

1. Chuẩn bị và hợp nhất dữ liệu đầu vào.
2. Tạo các đặc trưng phục vụ dự báo theo chuỗi thời gian.
3. Huấn luyện mô hình, sinh dự báo và giải thích kết quả dự đoán.

## Cấu trúc thư mục

- `03_Part3_Data_Prep.ipynb`: làm sạch, chuẩn hóa và tổng hợp dữ liệu đầu vào.
- `04_Part3_Feature_Eng.ipynb`: tạo lag features, rolling features và các biến hỗ trợ mô hình.
- `05_Part3_Modeling_SHAP.ipynb`: huấn luyện mô hình, tạo dự báo và phân tích SHAP.
- `requirements.txt`: danh sách thư viện cần cài.
- `shap_summary.png`: hình minh họa kết quả SHAP.
- `submissions/`: chứa file dự đoán cuối cùng dùng để nộp.

## Tôi đang làm gì trong phần này

- Xây dựng bộ dữ liệu theo thời gian từ dữ liệu nghiệp vụ đã xử lý ở Câu 2.
- Tạo các feature phản ánh xu hướng ngắn hạn, mùa vụ và ảnh hưởng của hoạt động kinh doanh.
- Huấn luyện mô hình dự báo cho từng ngày thay vì chỉ nhìn dữ liệu ở mức tổng hợp.
- Dùng SHAP để kiểm tra feature nào đang tác động mạnh nhất đến dự đoán.

## Quy trình chạy lại

### 1. Cài đặt thư viện

```bash
pip install -r requirements.txt
```

### 2. Chạy các notebook theo thứ tự

1. `03_Part3_Data_Prep.ipynb`
2. `04_Part3_Feature_Eng.ipynb`
3. `05_Part3_Modeling_SHAP.ipynb`

### 3. Kiểm tra kết quả

- File dự báo cuối cùng được lưu trong `submissions/`.
- Biểu đồ/đầu ra SHAP có thể được dùng để giải thích mô hình và kiểm tra tính hợp lý của dự báo.

## Ghi chú

- Cần chạy đúng thứ tự các notebook vì notebook sau phụ thuộc vào dữ liệu và feature được tạo ở notebook trước.
- Nếu thay đổi dữ liệu đầu vào, nên chạy lại toàn bộ pipeline để đảm bảo kết quả nhất quán.