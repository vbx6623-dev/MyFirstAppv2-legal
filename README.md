# MyFirstAppv2-legal (public)

Repo **chỉ chứa trang pháp lý** cho App Store — không có mã nguồn app.

## Tạo repo trên GitHub (một lần)

1. https://github.com/new
2. Tên repo: **`MyFirstAppv2-legal`**
3. Chọn **Public**
4. Không tick README / .gitignore
5. **Create repository**

## Push từ máy (PowerShell)

```powershell
cd "C:\Users\ADMIN\OneDrive\Desktop\opencode\MyFirstAppv2\legal-site"
git init
git add .
git commit -m "Initial legal pages for DN TUNING V2"
git branch -M main
git remote add origin https://github.com/vbx6623-dev/MyFirstAppv2-legal.git
git push -u origin main
```

## Bật GitHub Pages

1. Repo **MyFirstAppv2-legal** → **Settings** → **Pages**
2. Branch: **main**, Folder: **/ (root)**
3. Save

URL sau ~2 phút:

- https://vbx6623-dev.github.io/MyFirstAppv2-legal/support.html
- https://vbx6623-dev.github.io/MyFirstAppv2-legal/privacy-policy.html

## Cập nhật sau này

Sửa file HTML trong `legal-site/`, rồi:

```powershell
cd legal-site
git add .
git commit -m "Update legal pages"
git push
```

Repo **MyFirstAppv2** (app) có thể giữ **Private**.
