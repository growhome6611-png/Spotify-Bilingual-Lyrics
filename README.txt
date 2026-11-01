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
