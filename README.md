# Data Competition 2026 - Analysis & Forecasting

Dự án phân tích dữ liệu và dự báo doanh thu cho một nền tảng thương mại điện tử thời trang, gồm 3 phần chính: phân tích thống kê, tiền xử lý & EDA, và dự báo chuỗi thời gian với SHAP.

## Cấu trúc dự án

```
Data-compet/
├── Câu 1/              # Part 1: Statistical Analysis
│   ├── Q1.ipynb - Q10.ipynb    # 10 câu hỏi phân tích thống kê
│   ├── TongHopDapAn.txt        # Tổng hợp đáp án
│   └── README.md
│
├── Câu 2/              # Part 2: Data Preprocessing & EDA
│   ├── preprocessing.ipynb     # Làm sạch và chuẩn hóa dữ liệu
│   ├── EDA.ipynb               # Phân tích khám phá dữ liệu
│   ├── data/                   # Dữ liệu gốc
│   ├── cleaned_data/           # Dữ liệu đã xử lý
│   └── README.md
│
├── Câu 3/              # Part 3: Forecasting & SHAP
│   ├── 03_Part3_Data_Prep.ipynb           # Chuẩn bị dữ liệu
│   ├── 04_Part3_Feature_Eng.ipynb         # Tạo feature
│   ├── 05_Part3_Modeling_SHAP.ipynb       # Modeling & SHAP
│   ├── requirements.txt
│   ├── submissions/            # Dự báo cuối cùng
│   └── README.md
│
└── README.md           # File này
```

## Tổng quan từng phần

### Câu 1: Phân tích thống kê (Statistical Analysis)

Trả lời 10 câu hỏi phân tích dữ liệu về hành vi khách hàng, sản phẩm, doanh số bán hàng, lợi nhuận và các chỉ số kinh doanh khác. Mỗi câu hỏi được trình bày trong một notebook riêng với code, trực quan hóa và kết luận.

**Xem chi tiết:** [Câu 1/README.md](Câu%201/README.md)

### Câu 2: Tiền xử lý dữ liệu & EDA

Chuẩn bị dữ liệu sạch từ 13 bảng đầu vào bằng cách:
- Kiểm tra và xử lý dữ liệu thiếu, trùng lặp, định dạng sai.
- Chuẩn hóa kiểu dữ liệu và định dạng ngày tháng.
- Ghép các bảng liên quan để tạo dataset phân tích chung.
- Thực hiện EDA để khám phá pattern, trend và mối quan hệ.

Dữ liệu xử lý xong được lưu vào `cleaned_data/` để phục vụ các bước sau.

**Xem chi tiết:** [Câu 2/README.md](Câu%202/README.md)

### Câu 3: Dự báo & Giải thích SHAP

Xây dựng pipeline dự báo Revenue và COGS theo ngày cho giai đoạn 2023 - 2024 bằng:
- Tiền xử lý và tổng hợp dữ liệu chuỗi thời gian.
- Feature engineering: lag, rolling windows, web traffic trends.
- Modeling: ensemble giữa LightGBM và Prophet.
- Giải thích: SHAP values để phân tích tác động của từng feature.

Dự báo cuối cùng được lưu vào `submissions/` để nộp.

**Xem chi tiết:** [Câu 3/README.md](Câu%203/README.md)

## Cách chạy dự án

### 1. Clone/tải dự án

```bash
cd Data-compet
```

### 2. Tạo môi trường ảo (nếu chưa có)

```bash
python -m venv .venv
.venv\Scripts\activate  # trên Windows
# source .venv/bin/activate  # trên Linux/Mac
```

### 3. Chạy từng phần

**Câu 1:** Mở từng notebook Q1.ipynb đến Q10.ipynb và chạy các cell.

**Câu 2:**
```bash
cd Câu\ 2
jupyter notebook  # hoặc dùng VS Code
```
Chạy `preprocessing.ipynb` rồi `EDA.ipynb` theo thứ tự.

**Câu 3:**
```bash
cd Câu\ 3
pip install -r requirements.txt
jupyter notebook
```
Chạy 03, 04, 05 notebook theo thứ tự.

## Yêu cầu môi trường

- Python 3.8+
- Jupyter Notebook hoặc VS Code + Jupyter extension
- Các thư viện: pandas, numpy, scikit-learn, lightgbm, prophet, shap, matplotlib, seaborn

Chi tiết xem tại `Câu 3/requirements.txt`.

## Kết quả chính

- **Câu 1:** Tổng hợp đáp án 10 câu hỏi → [TongHopDapAn.txt](Câu%201/TongHopDapAn.txt)
- **Câu 2:** Dữ liệu sạch → [Câu 2/cleaned_data/](Câu%202/cleaned_data/)
- **Câu 3:** Dự báo CSV → [Câu 3/submissions/](Câu%203/submissions/)

## Liên hệ & Hỗ trợ

Nếu gặp lỗi khi chạy, vui lòng:
1. Kiểm tra các file dữ liệu có đầy đủ chưa.
2. Đảm bảo thư viện đã cài đặt đúng phiên bản.
3. Chạy lại các notebook từ đầu để đảm bảo tính nhất quán.
