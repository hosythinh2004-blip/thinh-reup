# Thinh Video Studio — thinh-reup

Kho GitHub dùng chung để phát triển, kiểm thử và đóng gói **Thinh Video Studio** trên Windows.

> Trạng thái: kho làm việc đã khởi tạo. **Mã nguồn v2.7 và file EXE chưa được tải lên kho này.**
> Chưa coi một bản phát hành là hoàn chỉnh nếu chưa kiểm thử Windows, PySide6, FFmpeg, NVIDIA (nếu dùng), tách giọng và lồng tiếng đồng bộ.

## Kết nối với Visual Studio Code

1. Cài Visual Studio Code: https://code.visualstudio.com/
2. Cài Git for Windows: https://git-scm.com/downloads/win
3. VS Code → **Ctrl+Shift+P** → **Git: Clone**.
4. Dán URL: `https://github.com/hosythinh2004-blip/thinh-reup.git`
5. Chọn thư mục trên máy, mở dự án, sau đó đăng nhập GitHub khi VS Code yêu cầu.
6. Khi chỉnh sửa: vào **Source Control → Commit → Sync Changes**.

Muốn sử dụng AI để sửa mã trong VS Code: cài tiện ích **Codex** qua Marketplace, đăng nhập tài khoản ChatGPT và mở thư mục repo này. Xem: https://developers.openai.com/codex/ide

## Nguyên tắc phát triển

- Sửa mã nguồn trên nhánh riêng, kiểm thử trước khi gộp về `main`.
- Không commit mật khẩu, cookie Chrome, API Key, token, .env, dữ liệu riêng tư.
- Không đưa các thư mục `.venv`, model AI nặng, video cá nhân hoặc file EXE không kiểm chứng lên repo.
- Khi có mã nguồn Python, thêm kiểm thử tự động trong `.github/workflows` trước khi phát hành.
- Mọi file EXE cuối cùng phải được build trên Windows và kiểm thử ít nhất khởi động, video mẫu, phụ đề, giọng đọc, render.

## Mục tiêu sản phẩm

Quy trình video đầu vào → ASR → dịch SMART FREE → tạo giọng → tách giọng và giữ âm nền → che phụ đề cũ / đè phụ đề mới → preview → xuất video.

**Lưu ý bảo mật:** Repository hiện công khai (public). Nếu muốn giữ kín mã nguồn, đổi sang **Private** trong Settings → General → Danger Zone → Change repository visibility.
