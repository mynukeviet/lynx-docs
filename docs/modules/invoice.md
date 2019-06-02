---
title: Quản lý hóa đơn
---

## Gửi thông tin hóa đơn

Sau khi tạo hóa đơn, nếu bạn cần gửi thông tin hóa đơn cho khách hàng qua email, thực hiện như sau: 

- Tại giao diện chi tiết hóa đơn, chọn **Gửi thông tin**
- Hệ thống sẽ gửi thông tin hóa đơn và file đính kèm hóa đơn ở định dạng file PDF qua email chính của khách hàng

!!! note "Ghi chú"
    Bạn có thể tùy chỉnh nội dung email thông báo thông tin hóa đơn, nội dung file PDF thông tin hóa đơn tại **ACP / Hóa đơn (menu dọc) / Cấu hình nội dung**

## Tự động tạo hóa đơn cho chu kỳ tiếp theo

Đối với các hóa đơn mang tính chất lặp đi lặp lại theo chu kỳ, bạn nên sử dụng tính năng này để hệ thống tự động tạo hóa đơn mới khi sắp hết hạn hóa đơn.

Để một hóa đơn được tạo theo chu kỳ mới, tại giao diện **thêm/sửa** hóa đơn, cần lưu ý phải có đủ các thông tin như mô tả bên dưới:

![](/images/tao-hoa-don-theo-chu-ky.png)

- Chọn Ngày bắt đầu hóa đơn (1)
- Chọn Chu kỳ thanh toán (2)
- Chọn Ngày kết thúc hóa đơn (3)
- Chọn Tự động tạo hóa đơn (4)

Với hóa đơn được thiết lập tạo tự động theo chu kỳ, hệ thống sẽ:

- **Tự động tạo hóa đơn** theo thông tin của chu kỳ mới
- **Trước 8 ngày** (tỉnh từ ngày kết thúc hóa đơn)
	- Gửi thông tin hóa đơn mới cho khách hàng qua email
	- Gửi thông báo cho người phụ trách hóa đơn
- **Trước 2 ngày** (tỉnh từ ngày kết thúc hóa đơn), nếu hóa đơn mới vấn chưa được thanh toán, hệ thống sẽ tự động gửi email nhắc thanh toán thêm một lần nữa.

## Thêm giao dịch

Một hóa đơn có thể có nhiều hơn một lần giao dịch (chia thành nhiều giai đoạn thanh toán). Với mỗi lần thanh toán, hệ thống sẽ hỗ trợ bạn ghi nhận các thông tin về lượt thanh toán đó (thời gian, trạng thái, số tiền,...)

Hướng dẫn thêm giao dịch

- Tại giao diện chi tiết hóa đơn, tìm đến khu vực **Lịch sử giao dịch**, chọn **Thêm giao dịch**
- Điền đầy đủ thông tin giao dịch, nhấn **Thêm giao dịch** để lưu thông tin

!!! note "Ghi chú"

    - Nếu số tiền giao dịch bằng hoặc lớn hơn giá trị hóa đơn, hệ thống tự động chuyển hóa đơn sang trạng thái **Đã thanh toán đủ**
    - Nếu số tiền nhỏ hơn giá trị hóa đơn, hệ thống tự động chuyển trạng thái hóa đơn sang **Đã thanh toán trước**

## Xác nhận thanh toán

Sau khi xác nhận hóa đơn đã được **thanh toán đủ** , người quản lý hóa đơn cần xác nhận rằng hóa đơn đã được thanh toán.

- Tại giao diện chi tiết hóa đơn, nhấn **Xác nhận thanh toán**
- Sau khi xác nhận thành công, hệ thống sẽ:
	- Tự động chuyển trạng thái hóa đơn sang **Đã thanh toán đủ**
	- Tự động gửi thông báo về trạng thái hóa đơn qua email cho khách hàng 

!!! note "Ghi chú"
    Bạn có thể tùy chỉnh nội dung email xác nhận thanh toán tại **ACP / Hóa đơn (menu dọc) / Cấu hình nội dung**, chọn tab **Nội dung xác nhận hóa đơn**

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