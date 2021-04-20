1. Nếu như ta xóa tag <activity> trong manifest thì điều gì sẽ xảy ra, vì sao ?
2. Khi các bạn tạo project mới sẽ thấy 2 folder trong res là values và values-night,
 tại sao lại có sự xuất hiện của 2 folder này ?
1:project sẽ không chạy được và sẽ hiển thị "Error running 'app': Default Activity not found"
bởi vì trong manifest là nơi hệ thống toàn bộ thông tin ứng dụng ví dụ như sử dụng internet, cấp quyền,...
trong phần <activity> sẽ được xem như là từng màn hình giao diện
với mỗi <activity> sẽ là 1 màn hình giao diện riêng
khi xóa đi sẽ coi như là không có màn hình giao diện nào

2: thư mục values chứa tất cả các tài nguyên trên app ví dụ như trong
các file color.xml strings.xml styles.xml
tác dụng đễ dễ dàng chỉnh sửa và truy cập các tài nguyên
