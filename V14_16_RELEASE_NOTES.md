# V14.16 — Google Drive auto reconnect

- Tự thử khôi phục phiên Google Drive bằng Google Identity Services khi khởi động, quay lại tab hoặc cửa sổ.
- Giữ trạng thái muốn kết nối; nút Ngắt kết nối tắt tự khôi phục và thu hồi token hiện tại nếu có.
- Khi token hết hạn hoặc Google API trả 401, thử cấp token mới thay vì xem đó là thao tác ngắt kết nối chủ động.
- Nút Kết nối Drive vẫn cho phép xác nhận quyền truy cập khi Google yêu cầu.
- Không thể đảm bảo đăng nhập vĩnh viễn: chính sách OAuth của Google, phiên trình duyệt, popup và consent có thể yêu cầu người dùng xác nhận lại.
- Giữ nguyên dữ liệu và các tính năng V14.15.
