# YÊU CẦU 1: FILE TIỀN XỬ LÝ DỮ LIỆU

Cần **1 file đầu tiên** để thực hiện tiền xử lý dữ liệu, bao gồm:

- Kiểm tra số dòng, số cột, kiểu dữ liệu của từng file.  
- Xử lý **missing values**.  
- Xử lý **duplicate records**.  
- Sửa lỗi **format ngày tháng**.  
- Chuyển đổi **sai kiểu dữ liệu số** về đúng định dạng.  

---

# YÊU CẦU 2: FILE THỰC HIỆN EDA

Cần **1 file riêng** để thực hiện **Exploratory Data Analysis (EDA)**:

- Merge các bảng quan trọng thành dataset dùng chung:  
  - `orders`  
  - `order_items`  
  - `products`  
  - `customers`  
  - `payments`  
  - `returns`  
  - `shipments`  

- Tạo các feature hỗ trợ phân tích:
  - Doanh thu  
  - Lợi nhuận gộp  
  - Return rate  
  - Delivery time  
  - Customer lifetime value  
  - Monthly sales  

- Lưu dữ liệu sạch thành file trung gian để nhóm **Visualization / Modeling** có thể sử dụng ngay.  

- Code rõ ràng, reproducible, có notebook/script riêng.  

- Join và merge nhiều bảng để tìm ra insights quan trọng thay vì chỉ phân tích từng bảng riêng lẻ.  

---

# YÊU CẦU 3: FILE THỰC HIỆN VISUALIZATION

Cần **1 file riêng** để trực quan hóa dữ liệu:

- Thiết kế và xây dựng:
  - Biểu đồ  
  - Đồ thị  
  - Bản đồ  
  - Dashboard  

- Mục tiêu:
  - Thể hiện patterns trong dữ liệu  
  - Tìm xu hướng (trends)  
  - Khám phá mối quan hệ ẩn sâu trong bộ dữ liệu mô phỏng doanh nghiệp thời trang  

---

# YÊU CẦU 4: FILE LATEX GIẢI THÍCH PHẦN VISUALIZATION

Sử dụng **1 file LaTeX** để giải thích từng phần trực quan hóa của **Yêu cầu 3**.

## Với mỗi biểu đồ cần có:

### 1. Mô tả

- Nêu rõ biểu đồ thể hiện gì.  
- Giải thích vì sao góc nhìn này quan trọng đối với doanh nghiệp.  

### 2. Phát hiện chính (Key Findings)

- Chỉ ra xu hướng nổi bật.  
- Phát hiện điểm bất thường.  
- Nêu các mối quan hệ được hỗ trợ bằng số liệu cụ thể.  

### 3. Đề xuất hành động (Actionable Recommendations)

- Giải thích ý nghĩa kinh doanh.  
- Đưa ra hành động cụ thể doanh nghiệp nên thực hiện.  
