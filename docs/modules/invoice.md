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

- Với trường hợp cần tải PDF để in ấn hoặc gửi thông tin cho khách hàng. Tại trang chi tiết hóa đơn, click chọn menu **Tùy chọn khác => Xuất file pdf**

![](/images/tai-hoa-don-pdf.png)

- Bạn có thể tùy chỉnh nội dung, giao diện file thông qua econtent (**ACP / Hóa đơn / Cấu hình gửi mail**) , chọn tab **Nội dung file pdf hóa đơn**

- Đối với [phiên bản Opensource](https://github.com/tdfoss/lynx), cần cài đặt thư viện Mpdf để sử dụng tính năng này

> composer require mpdf/mpdf

## Cấu hình sử dụng điểm tích lũy

Điểm tích lũy cho phép bạn cộng dồn điểm cho khách hàng ở mỗi lần giao dịch thành công (Thanh toán thành công hóa đơn). Số điểm này có thể quy ra tiền, sử dụng cho các lần thanh toán tiếp theo.

### Kích hoạt tính năng tích lũy điểm

Mặc định, tính năng này không được kích hoạt, để kích hoạt, bạn cần:

1. **Truy cập ACP / Hóa đơn / Cấu hình**
2. Check chọn **Sử dụng điểm tích lũy**
3. **Giá trị quy đổi 1 điểm (VNĐ)**, được tính sau khi thanh toán hóa đơn thành công, 1 điểm sẽ bằng bao nhiêu tiền, dựa trên tổng tiền hóa đơn để cộng điểm cho khách hàng
4. **Giá trị sử dụng 1 điểm (VNĐ)**, sử dụng khi thanh toán, nếu chọn thanh toán bằng điểm tích lũy, thì với số tiền cần thanh toán khách hàng sẽ bị trừ bao nhiêu điểm

Nhấn **Lưu thay đổi** để cập nhật cấu hình

### Sử dụng điểm tích lũy

- Điểm tích lũy sẽ được cộng dồn vào quỹ điểm của khách hàng với mỗi hóa đơn thanh toán thành công. Điểm tích lũy sẽ được sử dụng (trừ đi) khi khách hàng thanh toán một hóa đơn mới.
 
- Khi bạn **thêm một giao dịch** cho hóa đơn, hệ thống sẽ thông báo tổng số điểm mà khách hàng đang có

- Bạn có thể chủ động chọn hình thức thanh toán là **Tiền mặt**, hoặc **Điểm tích lũy**

![](/images/them-giao-dich.png)

### Điểm tích lũy toàn bộ khách hàng

- Trên giao diện quản lý, chọn **Hóa đơn (Menu dọc) => Điểm tích lũy**
- Tại giao diện này, hệ thống hiển thị danh sách dạng bảng, các thông tin như họ tên, email, điện thoại, điểm, thành tiền