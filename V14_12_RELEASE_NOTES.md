# V14.12 – Tên tệp dễ đọc và xem vị trí trên Drive

- Khi lưu lời bài hát mới, tên JSON có dạng `Tên bài - Ca sĩ__vi__lyrics.json`.
- Khi tự lưu bản dịch bài hiện tại, tên JSON có dạng `Tên bài - Ca sĩ__vi.json` nếu có đủ metadata; nếu không, dùng tên mã cũ để không ghi sai tên.
- Nút 📍 bên cạnh bài trong thư viện mở đúng tệp trên Google Drive.
- Nút `Đổi tên tệp cũ theo tên bài hát` đổi tên tệp JSON đang tồn tại mà không thay đổi nội dung hay ID Google Drive; tra cứu metadata đã ghi trên thiết bị hoặc Spotify khi có quyền truy cập. Không đoán tên nếu không tìm được, không đổi tên khi trùng.
- Đồng bộ tăng dần nhận diện các tệp đã đổi tên thông qua trackKey trong JSON, tránh tải lên tệp trùng.
- Tương thích tên mã cũ để khôi phục bản dịch.

Lưu ý: Các tệp cũ chỉ chứa mã trackKey, không có title/artist. Để đổi tên hàng loạt cần Spotify kết nối và quyền đọc thông tin bài hát; một số tệp không thể đổi tên nếu không tra cứu được metadata. Hãy sao lưu Drive trước khi chạy. Chưa kiểm thử OAuth Drive/Spotify thực tế.
