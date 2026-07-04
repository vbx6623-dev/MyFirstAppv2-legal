# MyFirstAppv2-legal (public)

Repo **chỉ chứa trang pháp lý & hỗ trợ** cho App Store — **không có mã nguồn app**.

| Trang | URL live |
|-------|----------|
| Trang chủ | https://vbx6623-dev.github.io/MyFirstAppv2-legal/ |
| Hỗ trợ | https://vbx6623-dev.github.io/MyFirstAppv2-legal/support.html |
| Quyền riêng tư | https://vbx6623-dev.github.io/MyFirstAppv2-legal/privacy-policy.html |
| Điều khoản | https://vbx6623-dev.github.io/MyFirstAppv2-legal/terms-of-use.html |

Repo app **MyFirstAppv2** có thể giữ **Private**.

---

## Tạo repo trên GitHub (một lần)

1. https://github.com/new
2. Tên: **`MyFirstAppv2-legal`**
3. **Public** · không tick README
4. Push nội dung thư mục `legal-site/` từ project app

---

## Bật GitHub Pages

1. Repo → **Settings** → **Pages**
2. **Source:** **GitHub Actions** (không dùng "Deploy from a branch")
3. Push lên `main` → tab **Actions** → workflow **Deploy GitHub Pages** (tick xanh)
4. **Visit site** xuất hiện trong Settings → Pages

Workflow: [`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml)

---

## Cập nhật sau này

Sửa HTML/CSS trong `legal-site/` (font: **Be Vietnam Pro** trong `assets/style.css`):

```powershell
cd "C:\Users\ADMIN\OneDrive\Desktop\opencode\MyFirstAppv2\legal-site"
git add .
git commit -m "Update legal pages"
git push origin main
```

GitHub Actions tự deploy — đợi 1–2 phút rồi refresh URL.

---

## Đồng bộ với app

URL trong app lấy từ [`app/constants/legal.ts`](../app/constants/legal.ts) và [`app.json`](../app.json) → `extra.privacyPolicyUrl`, `supportUrl`.

Sau khi đổi URL, cập nhật cả:
- `legal.ts`
- `app.json` → `extra`
- App Store Connect (Privacy Policy URL, Support URL)

---

## App Store Connect

| Trường | Giá trị |
|--------|---------|
| Privacy Policy URL | `…/privacy-policy.html` |
| Support URL | `…/support.html` |
| Support Email | vbx6623@gmail.com |
| Developer | Nguyễn Văn Dương |

Checklist đầy đủ: [docs/APP_STORE_SUBMISSION.md](../docs/APP_STORE_SUBMISSION.md)

---

*Cập nhật: 4 tháng 7, 2026*
