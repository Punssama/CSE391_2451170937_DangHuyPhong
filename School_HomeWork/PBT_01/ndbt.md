## PHẦN B — THỰC HÀNH CODE (60 điểm)

> ⚠️ **YÊU CẦU:**
> - Tạo folder `PBT_01/` trong repo Git
> - Mỗi bài tạo file riêng
> - **Commit sau mỗi bài** (không gộp commit)
> - Chụp screenshot kết quả trên browser

### Bài B1 (15đ) — Trang Profile cá nhân

Tạo file `profile.html` — trang giới thiệu bản thân với **đầy đủ semantic HTML5**:

**Yêu cầu bắt buộc:**
- [ ] `<!DOCTYPE html>`, `<html lang="vi">`, `<meta charset>`, `<meta viewport>`
- [ ] `<title>` chứa tên bạn
- [ ] `<header>` chứa `<nav>` với ít nhất 3 links nội bộ (dùng `#id`)
- [ ] `<main>` chứa ít nhất 2 `<section>`:
  - Section "Về tôi": `<article>` giới thiệu, có `<figure>` + `<figcaption>` chứa ảnh đại diện
  - Section "Kỹ năng": bảng `<table>` với header, body, footer — liệt kê ít nhất 5 kỹ năng + mức độ
- [ ] `<aside>` chứa thông tin liên hệ
- [ ] `<footer>` với copyright
- [ ] **KHÔNG DÙNG** bất kỳ thẻ `<div>` nào (ngoại trừ wrapper) — chỉ dùng semantic tags

**Bảng kỹ năng mẫu (nhưng bạn phải tự điền thông tin thật):**

| Kỹ năng | Mức độ | Ghi chú |
|---------|--------|---------|
| HTML | ⭐⭐ | Đang học |
| CSS | ⭐ | Mới bắt đầu |
| ... | ... | ... |

**Chấm điểm:**
- 5đ: Cấu trúc semantic đúng (header/nav/main/article/section/aside/footer)
- 5đ: Table đúng cấu trúc (thead/tbody/tfoot)
- 3đ: Meta tags đầy đủ (charset, viewport, title)
- 2đ: Không dùng div thừa

### Bài B2 (15đ) — Trang Sản phẩm E-Commerce

Tạo file `products.html` — trang danh sách sản phẩm:

**Yêu cầu bắt buộc:**
- [ ] Header + Navigation giống Bài B1 (có thể copy)
- [ ] Section "Sản phẩm nổi bật" chứa ít nhất **4 sản phẩm**, mỗi sản phẩm là 1 `<article>` bao gồm:
  - `<figure>` + `<img>` (dùng placeholder image: `https://placehold.co/300x200`)
  - `<h3>` tên sản phẩm
  - `<p>` mô tả ngắn
  - Giá: dùng `<strong>` hoặc `<mark>`
  - Link "Mua ngay" (dùng `<a>` trỏ đến `#`)
- [ ] Section "Bảng so sánh" — Table so sánh 3 sản phẩm cùng loại, có ít nhất 5 tiêu chí
- [ ] Table phải dùng `colspan` hoặc `rowspan` ít nhất 1 lần
- [ ] Footer chứa ít nhất 3 hyperlink (Chính sách, Liên hệ, FAQ)

**Chấm điểm:**
- 5đ: 4+ articles product card đúng cấu trúc
- 5đ: Table so sánh có colspan/rowspan
- 3đ: Hyperlinks hoạt động đúng (anchor links và external links)
- 2đ: Code indentation sạch, readable

### Bài B3 (15đ) — Debug HTML

File HTML dưới đây có **ít nhất 10 lỗi** (cả syntax lẫn semantic). Tìm và sửa TẤT CẢ.

Tạo file `debug.html` cho bản sửa. Trong `answers.md`, liệt kê từng lỗi theo format:
```
Lỗi 1: Dòng X — Mô tả lỗi — Cách sửa
Lỗi 2: ...
```

```html
<!DOCTYPE>
<html>
<head>
    <title>Trang web
    <meta charset="utf8">
</head>
<body>
    <h1>Welcome to ShopTLU<h1>
    
    <header>
        <nav>
            <a href="home">Trang chủ<a>
            <a href="products">Sản phẩm</a>
        </nav>
    </header>
    
    <main>
        <section>
            <h3>Sản phẩm hot</h3>
            <img src=iphone.jpg>
            <p>iPhone 16 Pro</p>
            <p>Giá: <b>25.990.000đ</p></b>
        </section>
        
        <section>
            <h3>Thông tin</h3>
            <table>
                <tr>
                    <td>Tên</td>
                    <td>Giá</td>
                </tr>
                <tr>
                    <td>iPhone</td>
                    <td>25tr</td>
                </tr>
            </table>
        </section>
    </main>
    
    <main>
        <p>Sidebar content</p>
    </main>
    
    <footer>
        <p>Copyright 2026
    </footer>
</body>
```

### Bài B4 (15đ) — Phân tích trang web thật

Chọn **1 trong 3 trang web** sau: `tiki.vn`, `shopee.vn`, `thegioididong.com`

Sử dụng DevTools (F12):

1. **Chụp screenshot** tab Elements, chỉ ra ít nhất:
   - 3 thẻ semantic HTML5 mà trang đó sử dụng (ghi rõ thẻ gì, ở đâu)
   - 2 thẻ mà trang đó KHÔNG dùng đúng semantic (nếu có)

2. Mở tab **Elements**, tìm 1 `<table>` trên trang. Chụp screenshot và trả lời:
   - Table đó hiển thị nội dung gì?
   - Có dùng `<thead>`, `<tbody>` không?

3. Tìm 1 `<form>` trên trang (ví dụ ô tìm kiếm). Chụp screenshot:
   - Form đó có `action` và `method` gì?
   - Input types nào được dùng?

**Tổng hợp trong `answers.md`** kèm tất cả screenshots trong folder `screenshots/`.

---
