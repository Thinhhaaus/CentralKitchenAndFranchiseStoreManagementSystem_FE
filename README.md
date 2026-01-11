# Central Kitchen and Franchise Store Management System

## 📌 Overview
**Central Kitchen and Franchise Store Management System** là hệ thống quản lý toàn diện nhằm kết nối **Bếp Trung Tâm (Central Kitchen)** và **các cửa hàng Franchise**, hỗ trợ quy trình đặt hàng – sản xuất – phân phối – theo dõi – báo cáo một cách hiệu quả, minh bạch và theo thời gian thực.

Hệ thống được thiết kế theo **mô hình phân quyền theo vai trò (Role-based Access Control)**, mỗi actor có dashboard và chức năng riêng, phù hợp với nghiệp vụ thực tế trong chuỗi F&B.

---

## 🎯 Mục tiêu hệ thống
- Chuẩn hóa quy trình đặt hàng và cung ứng giữa Franchise và Central Kitchen
- Tối ưu kế hoạch sản xuất và phân phối
- Giảm hao hụt nguyên liệu, kiểm soát hạn sử dụng và tồn kho
- Cung cấp báo cáo và phân tích hiệu suất cho quản lý
- Tăng tính minh bạch và khả năng kiểm soát toàn hệ thống

---

## 🧑‍💼 Actors & Responsibilities

### 1️⃣ Franchise Store Staff
**Vai trò:** Nhân viên cửa hàng Franchise  

**Chức năng chính:**
- Tạo đơn đặt hàng nguyên liệu / bán thành phẩm từ bếp trung tâm
- Theo dõi trạng thái xử lý và giao hàng của đơn đặt
- Xác nhận đã nhận hàng và phản hồi chất lượng
- Xem tồn kho hiện tại tại cửa hàng

---

### 2️⃣ Central Kitchen Staff
**Vai trò:** Nhân viên bếp trung tâm  

**Chức năng chính:**
- Tiếp nhận và xử lý đơn đặt hàng từ các cửa hàng franchise
- Lập kế hoạch sản xuất theo nhu cầu tổng hợp
- Cập nhật trạng thái sản xuất và xuất kho
- Quản lý nguyên liệu đầu vào, hạn sử dụng và lô sản xuất

---

### 3️⃣ Supply Coordinator
**Vai trò:** Điều phối cung ứng  

**Chức năng chính:**
- Tổng hợp và phân loại đơn đặt hàng từ các cửa hàng
- Điều phối sản xuất và phân phối hàng hóa
- Lập lịch giao hàng và theo dõi tiến độ vận chuyển
- Xử lý các vấn đề phát sinh (thiếu hàng, giao trễ, hủy đơn)

---

### 4️⃣ Manager
**Vai trò:** Quản lý vận hành  

**Chức năng chính:**
- Quản lý danh mục sản phẩm, công thức và định mức nguyên liệu
- Quản lý tồn kho bếp trung tâm và cửa hàng
- Theo dõi hiệu suất sản xuất, phân phối và bán hàng
- Thống kê, báo cáo chi phí, hao hụt và hiệu quả vận hành

---

### 5️⃣ Admin
**Vai trò:** Quản trị hệ thống  

**Chức năng chính:**
- Quản lý người dùng và phân quyền theo vai trò
- Cấu hình hệ thống (đơn vị tính, quy trình, tham số vận hành)
- Quản lý danh mục cửa hàng franchise và bếp trung tâm
- Báo cáo tổng hợp toàn hệ thống

---

## 🔁 Business Workflow

```text
Franchise Store
    ↓ (Create Order)
Supply Coordinator
    ↓ (Aggregate & Schedule)
Central Kitchen
    ↓ (Produce & Dispatch)
Delivery
    ↓ (Ship & Track)
Franchise Store
    ↓ (Confirm & Feedback)
Manager / Admin
    ↓ (Monitor & Report)
