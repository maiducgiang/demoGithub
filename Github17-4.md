

Khi khởi tạo git(git init ), git sẽ tạo 1 folder .git. Mọi người cho biết tác dụng của folder này là gì? Giả sử, nếu xoá hoặc di chuyển folder này sang 1 thư mục khác thì điều gì sẽ xảy ra. Giải thích tại sao?

    folder .git: khiến project trở thành một git repository.
	 là thư mục con chứa thông tin git lưu trữ và thao tác: server liên kết với project,
	 lịch sử các lần commit, cấu trúc toàn bộ repository,
	 tập các script chạy tự động trước hoặc sau khi git thực hiện các câu lệnh quan trọng như commit, push,...
    Nếu xoá hoặc di chuyển folder này sang 1 thư mục khác, thì dữ liệu trong thư mục gốc vẫn giữ nguyên.
	nhưng không thể thực hiện các lệnh git đối với thư mục này.
    Xóa hoặc di chuyển folder .git sang thư mục khác, sẽ xóa các thông tin về các liên kết.
	 thao tác và các phiên bản đã commit mà git lưu trữ => thư mục cũ không còn là một git repository.

