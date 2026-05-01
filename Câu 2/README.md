# Câu 2 - Data Preprocessing & EDA

Mục tiêu của phần này là chuẩn bị dữ liệu đầu vào sạch, nhất quán và đủ cấu trúc để phục vụ cho các bước phân tích, trực quan hóa và modeling ở các phần sau.

## Tôi đang làm gì trong Câu 2

1. Kiểm tra và làm sạch dữ liệu gốc trong thư mục `data/`.
2. Chuẩn hóa kiểu dữ liệu, định dạng ngày tháng, giá trị thiếu và dữ liệu trùng lặp.
3. Ghép các bảng liên quan để tạo bộ dữ liệu phân tích chung.
4. Thực hiện EDA để tìm insight quan trọng về doanh thu, đơn hàng, khách hàng và vận hành.
5. Lưu dữ liệu đã xử lý vào `cleaned_data/` để các notebook khác có thể dùng lại ngay.

## Các file chính

- `preprocessing.ipynb`: làm sạch, chuẩn hóa và xuất dữ liệu đã xử lý.
- `EDA.ipynb`: phân tích khám phá dữ liệu, tạo feature và rút ra insight.
- `data/`: dữ liệu gốc ban đầu.
- `cleaned_data/`: dữ liệu sau tiền xử lý.

## Phạm vi xử lý

Trong phần này, tôi tập trung vào các bảng dữ liệu liên quan đến khách hàng, đơn hàng, sản phẩm, thanh toán, trả hàng, vận chuyển và các bảng nghiệp vụ khác để xây dựng một dataset thống nhất cho phân tích.

## Kết quả mong đợi

- Dữ liệu sạch, nhất quán và có thể tái sử dụng.
- Một bộ feature hữu ích cho phân tích và modeling.
- Các insight ban đầu về hành vi khách hàng, hiệu quả bán hàng và hiệu suất vận hành.
