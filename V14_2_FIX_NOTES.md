# V14.2 – sửa bài tập và chọn lời

- Sửa lỗi nghiêm trọng: mã bài tập V14.1 bị đặt bên trong thẻ script tải Google bên ngoài nên trình duyệt không chạy mã này. Chuyển vào script chính, sau khi khởi tạo biến giao diện.
- Sửa thuật toán đối chiếu tên bài/ca sĩ có chữ Hán, tăng trọng số thời lượng, từ chối kết quả khớp yếu.
- Lưu nguồn LRCLIB đã chọn để dùng lại.
- Lời TXT không còn được gán mốc thời gian giả mỗi 5 giây.
- Thay cache service worker để tải phiên bản mới.

Lưu ý: Không thể bảo đảm nguồn LRCLIB có cùng lời với Spotify, vì Spotify không cung cấp lời qua Web API. Nếu kết quả không khớp, cần dùng lời LRC được phép sử dụng và chọn thủ công. Chưa kiểm thử Spotify OAuth/phát nhạc thực tế.
