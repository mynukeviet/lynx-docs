---
title: Bắt đầu
---

## Về Lynx CMR

**Lynx CMR - Là một hệ thống quản trị quan hệ khách hàng (Customer Relationship Management)** được phát triển trên nền tảng [**CMS NukeViet**](https://nukeviet.vn/vi/about/gioi-thieu-ve-nukeviet.html), phát hành miễn phí theo giấy phép GNU (tiếng Anh: GNU General Public License, viết tắt GNU GPL hay chỉ GPL).

Lynx cung cấp các công cụ cơ bản, giúp việc quản lý nguồn dữ liệu doanh nghiệp khoa học, đơn giản hơn. Đặc biệt, với giấy phép GNU, bạn hoàn toàn có thể chỉnh sửa, phân phối mã nguồn này cho các mục đích khác nhau. Song, phải tôn trọng quyền tác giả bằng cách giữ lại các ghi chú về tác giả.

## Tải về mã nguồn Lynx

Để sở hữu mã nguồn Lynx, truy cập [Github](https://github.com/tdfoss/lynx/releases) để tải về phiên bản mới nhất trong danh sách.

## Yêu cầu máy chủ

- PHP: 5.6+
- MySQL: 5.5+
- PHP extensions (PDO, Opendir, GD, MCRYPT, Session)

## Cài đặt Lynx

## Cấu hình tiến trình tự động

Lynx sử dụng cronjobs để thực hiện một số công việc tự động. Bạn cần cấu hình cronjobs ở phía máy chủ (hosting) để đảm bảo hệ thống hoạt động thông suốt. Bạn cần thêm 2 cronjobs theo thông tin dưới đây:

```
*	*	*	*	*	curl -s "domain/index.php?second=cronjobs" > /dev/null 2>&1
```

```
*	*	*	*	*	sleep 10; curl -S "domain/sendmail.php" > /dev/null 2>&1
```

**Trong đó:**

- `*	*	*	*	*` quy định cronjobs sẽ thực thi mỗi phút một lần
- `sleep 10;` quy định 10 giây cronjobs sẽ thực thi mỗi phút một lần
- **domain** là tên miền đang chạy hệ thống. **Ví dụ:** lynx.vn, tdfoss.vn,.... 