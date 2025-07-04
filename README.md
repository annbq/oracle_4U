# Oracle Database 19c: Data Guard Administration Workshop

## 📘 Giới thiệu

Khóa học **Oracle Database 19c: Data Guard Administration** cung cấp kiến thức và kỹ năng cần thiết để quản trị, cấu hình và giám sát Oracle Data Guard – một tính năng quan trọng giúp đảm bảo khả năng phục hồi thảm họa và tính sẵn sàng cao cho cơ sở dữ liệu Oracle.

## 🎯 Mục tiêu khóa học

Sau khi hoàn thành workshop này, bạn sẽ có khả năng:

- Hiểu kiến trúc và các thành phần chính của Oracle Data Guard
- Cấu hình Data Guard theo chế độ Physical Standby và Active Data Guard
- Quản lý quá trình đồng bộ hóa và chuyển đổi vai trò (Role Transition)
- Giám sát và khắc phục sự cố Data Guard
- Thực hiện chuyển đổi vai trò (switchover/failover) theo cách thủ công và tự động

## 🛠️ Yêu cầu hệ thống

- **Oracle Database 19c** đã cài đặt trên cả Primary và Standby
- Hệ điều hành: Oracle Linux hoặc tương đương (REHL, CentOS)
- Cấu hình mạng: Các node có thể kết nối nhau qua `tnsnames.ora` hoặc dịch vụ listener
- SSH đã cấu hình giữa các node để thực hiện remote copy/log

## 🧱 Cấu trúc nội dung

### 1. Tổng quan Oracle Data Guard
- Kiến trúc và thành phần
- Physical Standby vs Logical Standby
- Mô hình đồng bộ (Synchronous vs Asynchronous)

### 2. Cài đặt và cấu hình Data Guard
- Chuẩn bị môi trường
- Cấu hình redo transport và log apply services
- Tạo Standby database bằng RMAN hoặc DBCA

### 3. Quản trị Data Guard
- Start/stop log apply
- Cấu hình redo transport mode
- Bảo trì tệp cấu hình và tham số

### 4. Chuyển đổi vai trò
- Switchover: planned role reversal
- Failover: automatic/manual
- Flashback sau failover

### 5. Giám sát và khắc phục sự cố
- Sử dụng `DGMGRL` và Enterprise Manager
- Kiểm tra cấu hình và trạng thái
- Khắc phục lỗi cấu hình mạng, redo, lag apply

## 🧪 Bài thực hành (Labs)

- **Lab 1**: Tạo Standby bằng RMAN DUPLICATE
- **Lab 2**: Kiểm tra và quản lý log shipping
- **Lab 3**: Switchover và Failover
- **Lab 4**: Giám sát bằng `dgmgrl` và Enterprise Manager

## 📂 Tài nguyên đi kèm

- Slide PDF khóa học
- Script cấu hình mẫu (listener.ora, tnsnames.ora, init.ora)
- Tài liệu chính thức từ Oracle: [Oracle Data Guard Documentation 19c](https://docs.oracle.com/en/database/oracle/oracle-database/19/dgbkr/index.html)

## ✅ Khuyến nghị

- Nên thử nghiệm trong môi trường LAB trước khi triển khai vào hệ thống thực
- Kết hợp với Oracle Recovery Manager (RMAN) để đảm bảo khôi phục toàn diện

---

> **© 2025 Oracle & Community Contributors.** Tài liệu chỉ dùng cho mục đích đào tạo và học tập. Không sử dụng cho hệ thống production khi chưa được kiểm thử đầy đủ.
