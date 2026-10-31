SPOTIFY BILINGUAL LYRICS - HUONG DAN DEPLOY VERCEL

1. Dua TOAN BO cac file va thu muc trong goi nay len mot GitHub repository.
2. Vao Vercel -> Add New Project -> Import repository -> Deploy.
3. Lay URL Vercel, vi du: https://spotify-bilingual-lyrics.vercel.app/
4. Vao Spotify Developer Dashboard -> App -> Settings -> Redirect URIs.
5. Them CHINH XAC URL Vercel o buoc 3, bao gom duong dan neu co.
6. Mo app -> Cai dat -> nhap Spotify Client ID va Google Cloud Translation API Key.
7. Bam Ket noi Spotify va chap nhan quyen.

LUU Y:
- Khong mo index.html bang file:/// vi Spotify OAuth khong chay trong che do nay.
- Neu test local, dung loopback server va dang ky Redirect URI tuong ung.
- Nen gioi han Google API key theo HTTP referrer/domain Vercel cua ban.
- PWA chi cache giao dien. Spotify, lyric va dich van can Internet.


V3: thêm Tìm kiếm, Thư viện Spotify, Playlist/Bộ sưu tập. Sau khi deploy bản V3, ngắt kết nối rồi kết nối Spotify lại để cấp các scope mới.
