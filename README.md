# CAB System – Bước 1: Tìm hiểu nghiệp vụ

## 1. Hệ thống hiện tại có những vấn đề gì?

Công ty ABC hiện đang cung cấp dịch vụ đặt xe thông qua tổng đài và một ứng dụng đơn giản. Tuy nhiên, hệ thống hiện tại còn tồn tại nhiều hạn chế:

### 1.1. Phân công tài xế thủ công

Việc phân công tài xế chủ yếu được thực hiện thủ công.

Điều này có thể dẫn đến:

- Mất nhiều thời gian để tìm tài xế.
- Khó lựa chọn tài xế phù hợp và gần khách hàng.
- Khó xử lý khi tài xế từ chối hoặc không phản hồi.
- Khó mở rộng khi số lượng khách hàng và tài xế tăng.

### 1.2. Khách hàng khó theo dõi chuyến đi

Khách hàng chưa có đầy đủ thông tin về trạng thái chuyến đi.

Khách hàng cần biết:

- Yêu cầu đặt xe đã được tiếp nhận hay chưa.
- Hệ thống đang tìm tài xế hay chưa.
- Tài xế nào đã nhận chuyến.
- Tài xế đang ở đâu.
- Thời gian dự kiến tài xế đến.
- Chuyến đi đang ở trạng thái nào.

### 1.3. Thông tin thanh toán chưa được quản lý tập trung

Thông tin thanh toán chưa được quản lý tập trung trong một hệ thống.

Do đó cần có cơ chế:

- Tính cước chuyến đi.
- Quản lý trạng thái thanh toán.
- Hỗ trợ tiền mặt.
- Hỗ trợ thanh toán điện tử.
- Xử lý khi thanh toán điện tử thất bại.
- Tra cứu lịch sử giao dịch.

### 1.4. Khó khăn trong vận hành

Bộ phận vận hành gặp khó khăn khi số lượng khách hàng và tài xế tăng.

Các vấn đề bao gồm:

- Khó quản lý tài xế.
- Khó quản lý phương tiện.
- Khó theo dõi các chuyến đang diễn ra.
- Khó xử lý các chuyến bị lỗi.
- Khó tra cứu lịch sử giao dịch.
- Khó kiểm soát quyền của từng nhân viên.

### 1.5. Khả năng mở rộng còn hạn chế

Hệ thống hiện tại chưa đáp ứng tốt nhu cầu phát triển lâu dài.

Doanh nghiệp cần khả năng:

- Phục vụ số lượng lớn khách hàng.
- Phục vụ số lượng lớn tài xế.
- Thêm loại dịch vụ mới.
- Thêm phương thức thanh toán.
- Thêm kênh thông báo.
- Thay đổi nhà cung cấp dịch vụ bên ngoài.
- Mở rộng từng thành phần của hệ thống độc lập.

### 1.6. Thiếu khả năng tự động hóa

Một số hoạt động quan trọng chưa được tự động hóa đầy đủ:

- Tìm tài xế.
- Phân công tài xế.
- Theo dõi trạng thái chuyến.
- Gửi thông báo.
- Tính cước.
- Xử lý thanh toán.
- Báo cáo hoạt động.

---

# 2. Mục tiêu của hệ thống mới

CAB System được xây dựng nhằm giải quyết các hạn chế của hệ thống hiện tại và tạo ra một nền tảng đặt xe có khả năng phát triển lâu dài.

## 2.1. Mục tiêu kinh doanh

- Xây dựng nền tảng đặt xe trực tuyến hiện đại.
- Giảm sự phụ thuộc vào việc phân công tài xế thủ công.
- Nâng cao trải nghiệm của khách hàng.
- Hỗ trợ nhân viên vận hành quản lý tập trung.
- Nâng cao hiệu quả hoạt động của tài xế.
- Có dữ liệu để theo dõi và đánh giá hoạt động kinh doanh.
- Có khả năng phục vụ số lượng lớn khách hàng và tài xế.
- Tạo nền tảng có khả năng mở rộng trong tương lai.

## 2.2. Mục tiêu hệ thống

Hệ thống mới cần hỗ trợ toàn bộ quy trình:

```text
Khách hàng đặt xe
        ↓
Tiếp nhận yêu cầu
        ↓
Tìm tài xế phù hợp
        ↓
Phân công tài xế
        ↓
Tài xế nhận chuyến
        ↓
Tài xế đến điểm đón
        ↓
Đón khách
        ↓
Thực hiện chuyến
        ↓
Hoàn thành chuyến
        ↓
Tính cước
        ↓
Thanh toán
        ↓
Đánh giá tài xế
