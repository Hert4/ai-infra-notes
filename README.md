# Nghiên cứu hạ tầng AI — MISA AI Platform

Trang tĩnh, không build, không generator. GitHub Pages phục vụ thẳng file.

```
index.html                  danh sách bài
assets/site.css             toàn bộ style, dùng chung
posts/<slug>/index.html     một bài
posts/<slug>/img/*.jpg      ảnh của bài đó
```

## Đăng bài mới

1. `cp -r posts/nhanh-bay-lan-khong-them-gpu posts/<slug-moi>` rồi thay nội dung
   trong `index.html` và ảnh trong `img/`. Giữ nguyên phần `<nav>` và `<footer>`.
2. Mở `index.html` ở thư mục gốc, sửa khối `<!-- BÀI MỚI NHẤT -->` trỏ sang bài mới,
   và thêm một `<li>` vào khối `<!-- KHO BÀI -->`.
3. Commit, push. Pages tự cập nhật sau khoảng một phút.

Xem thử tại chỗ: `python3 -m http.server -d . 8000`

## Quy ước

- Cột chữ 640px, ảnh 950px, ảnh không đóng khung.
- Ảnh nén JPEG chất lượng 88, cạnh dài tối đa 1400px.
- Không đưa flag và giá trị tuning của cấu hình serving lên bài.
