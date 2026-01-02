# BASCookies

Tool quản lý cookies cho BAS (Browser Automation Studio) - Lấy và nạp cookies từ browser thật.

## Tải về

| Platform | Download |
|----------|----------|
| Windows | [bascookies-windows.exe](https://github.com/TechScapBot/cookies-releases/releases/latest/download/bascookies-windows.exe) |
| macOS | [bascookies-macos.zip](https://github.com/TechScapBot/cookies-releases/releases/latest/download/bascookies-macos.zip) |

### Hướng dẫn cài đặt macOS
1. Tải file `bascookies-macos.zip`
2. Giải nén (double-click) để được `bascookies-macos.app`
3. Mở **Terminal** và chạy lệnh sau để bỏ chặn app:
   ```bash
   xattr -cr ~/Downloads/bascookies-macos.app
   ```
4. Double-click vào `bascookies-macos.app` để mở

> **Lưu ý:** Nếu bạn giải nén app vào thư mục khác, hãy thay đổi đường dẫn trong lệnh cho phù hợp.

---

## Hướng dẫn sử dụng nhanh

### 1. Lấy Cookies từ Browser

1. Mở tool BASCookies
2. Nhập **Domain** (ví dụ: `gmail.com`, `poe.com`)
3. Nhập **ID Request** (ID định danh cho account, ví dụ: `account_001`)
4. Nhấn **"Mở Browser"**
5. Đăng nhập vào tài khoản trong browser mở ra
6. Sau khi đăng nhập xong, **đóng browser**
7. Cookies sẽ tự động được lưu

### 2. Nạp Cookies vào Browser

1. Mở tool BASCookies
2. Nhập **Domain** và **ID Request** giống lúc lấy cookies
3. Nhấn **"Tải Cookies từ Server"** để lấy cookies đã lưu
4. Nhấn **"Nạp Cookies"** để mở browser với cookies đã lưu
5. Browser sẽ mở và tự động đăng nhập

### Lưu ý quan trọng

- **ID Request phải unique** cho mỗi tài khoản
- **Cùng ID Request** = Cùng profile browser = Không bị logout
- Mỗi máy tính cần lấy cookies riêng (profile browser không share được giữa các máy)

---

## Changelog

### v1.1.2 (2026-01-02)
- Thông báo toast hiển thị domain thay vì ID Request
- Sửa màu thông báo dừng batch từ đỏ sang xanh
- Cải thiện khoảng cách UI cho batch list

### v1.1.1 (2025-01-02)
- Fix Cloudflare detection
- Profile per ID Request để tránh logout

### v1.1.0 (2025-01-01)
- Thêm tính năng Profile per ID Request
- Anti-detection cho Gmail và Cloudflare
- Hỗ trợ đa domain

---

**Developed by ScapBot**
