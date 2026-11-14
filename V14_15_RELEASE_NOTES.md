# V14.15 - Gộp nhập LRC mở rộng
- Giao diện nhập nhạc chỉ còn hai mục: tệp âm thanh và một tệp LRC mở rộng chứa lời gốc, Pinyin, bản dịch.
- Giữ bộ đọc LRC mở rộng `[py]`, `[tr]` đã có; quét LRC trên máy và Drive tiếp tục điền vào cùng mục LRC.
- Nút lưu bộ tệp Drive tải lên nhạc và LRC (không tải bản dịch rời trong thao tác mới).
- Đầu vào bản dịch rời được ẩn nhưng vẫn duy trì để đọc các manifest Drive cũ; chỉ áp dụng khi tệp lời chưa có bản dịch.
- Không xóa hoặc chuyển đổi dữ liệu JSON hiện có.
- Chưa thử OAuth Google Drive và PWA trên thiết bị thật.
