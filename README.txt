Spotify Bilingual Lyrics V5

Nang cap:
- Spotify Web Playback SDK: phat nhac truc tiep trong app
- Play/Pause, Previous, Next, seek, volume
- Tim kiem, Thu vien, Playlist/BST
- Lyrics dong bo va dich song ngu

YEU CAU:
1. Deploy tren HTTPS/Vercel.
2. Redirect URI trong Spotify Developer Dashboard phai trung URL app.
3. Sau khi cap nhat V5, ngat ket noi Spotify va ket noi lai de cap them scope streaming + user-modify-playback-state.
4. Web Playback SDK yeu cau tai khoan Spotify Premium.
5. Tren iPhone, sau khi chuyen thiet bi phat co the can cham nut Play mot lan.


V8: thêm thanh điều hướng đáy kiểu Spotify và Google Drive Sync cho bản dịch. Cần tạo Google OAuth Client ID loại Web application, thêm domain Vercel vào Authorized JavaScript origins, bật Google Drive API, và dùng scope drive.file.

V11.1: Spotify API limit 10 for search, playlists, albums, library and following; next-page requests clamped to 10.

V11.9 (2026-11-02)
- Khôi phục bảng Google Drive Sync đầy đủ vào cửa sổ Cài đặt.
- Sửa cửa sổ cài đặt cuộn độc lập, giới hạn chiều cao theo màn hình điện thoại.
- Nút Lưu và Đóng luôn nằm trong cửa sổ, tránh bị thanh điều hướng che.
- Giữ nguyên các ID và hàm đồng bộ của V11.8, không xóa dữ liệu cục bộ.

V11.13 - LUYEN TAP QUA LOI BAI HAT
- Nhan nut mu tot nghiep (🎓) tren thanh dieu khien.
- Tao 5/10/20 cau: dien tu, trac nghiem, sap xep, nghe chep chinh ta.
- Tao tu dong tren thiet bi khong can API, hoac chon AI Gemini va nhap Gemini API key.
- Cho phep them, sua, xoa cau hoi, cham diem va luu ket qua tren thiet bi.
- Nut Dong bo bai tap: luu tai tep JSON rieng trong thu muc Spotify Bilingual Lyrics tren Drive.
- Neu phat hien ban tren Drive khac voi may, ung dung khong ghi de tu dong.
- Phat lai doan nhac yeu cau Spotify Premium, ket noi hop le va loi co moc thoi gian.
- Khong thay doi du lieu loi bai hat va ban dich hien co.

V11.15: Playback controls now target active Spotify Connect device via Web API; fixes idle Web SDK no-list-loaded error.
