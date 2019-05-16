---
title: Quản lý hóa đơn
---

## Báo cáo doanh thu, lợi nhuận

- Truy cập menu Hóa đơn / Báo cáo
- Biểu đồ line thống kê
	- **Doanh thu:** số liệu thu từ hóa đơn, danh sách thu (Văn phòng / Quản lý thu chi / Danh sách thu)
	- **Chi:** số liệu từ danh sách chi (Văn phòng / Quản lý thu chi / Danh sách chi)
	- **Lợi nhuận:** Lợi nhuận = Doanh thu - Chi 

## Bình luận trong hóa đơn

Tính năng này giúp các nhân viên có thể thảo luận về hóa đơn ngay tại trang xem chi tiết hóa đơn. 

Để bật tính năng này, **ACP / Quản lý bình luận / Cấu hình**. Chọn **Sửa** ở module **Hóa đơn**, tích chọn vào **Sử dụng chức năng bình luận** và **Lưu cấu hình**

Quay lại xem chi tiết hóa đơn, cuối trang sẽ xuất hiện khu vực bình luận

## Tải hóa đơn PDF

Đối với phiên bản Opensource, cần cài đặt thư viện PHP MPDF để cố thể tải về hóa đơn PDF

> composer require mpdf/mpdf