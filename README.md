# 📖 Book & Quote Mockup Studio (Trình Tạo Trang Sách & Quote Giả Lập)

Một ứng dụng web **Single-file (1 file HTML duy nhất)** mô phỏng trực quan các trang sách in văn học, bản thảo máy đánh chữ và quote vuông nghệ thuật (chuẩn style Wattpad / BookTok / Threads). 

Chỉnh sửa văn bản trực tiếp theo thời gian thực (*WYSIWYG*), tự động căn chỉnh dàn trang chuẩn xuất bản và xuất ảnh độ phân giải cực cao (Ultra-HD / 4K) không bể hạt.

---

## ✨ Tính Năng Nổi Bật

### 1. Hai Chế Độ Linh Hoạt (Dual Modes)
- **📄 Khổ Trang Sách Dài:** Dành cho viết tiểu thuyết, tản văn, có running-head (tên sách / tác giả hai bên), tiêu đề chương lớn, thụt đầu dòng, phân cảnh `* * *` và số trang.
- **🔲 Quote Vuông 1:1:** Chuẩn khổ ảnh vuông đăng Instagram, Facebook, Threads, TikTok với dấu ngoặc kép giọt nước đôi (*Playfair Display*) đặc trưng.

### 2. Định Dạng In Ấn & Chú Thích Thông Minh
- **Đánh số chú thích mũ chân trang (`¹`, `²`, `³`):** Chỉ cần gõ số thường (1, 2, 3...) hệ thống tự động đổi thành số mũ và thêm dòng giải nghĩa dàn ngang chân trang.
- **Drop Cap (Chữ to đầu dòng):** Phóng to chữ cái mở đầu chương chuẩn tiểu thuyết kinh điển.
- **Highlight thông minh (Vàng / Xám / Gạch đỏ nét bút):** Bôi đen bấm để tô, bấm lại lần 2 để hủy. Thuật toán render tách lớp chống tràn màu và không che dấu móc chữ (`ư`, `ơ`, `?`).

### 3. Hiệu Ứng Bề Mặt & Chữ Nghệ Thuật (Studio Effects)
- **🖋️ Mực lem (Ink Bleed):** Mô phỏng mực ngấm loang vào xơ giấy bằng ma trận toán học vi hạt SVG (`feTurbulence` seed 6).
- **💧 Mực ướt (Wet Ink):** Tạo cảm giác chữ đậm đà, óng ánh như vừa viết bằng bút máy Pilot/Parker.
- **🧱 Chữ ép dập chìm (Letterpress):** Tạo gờ sáng/tối như khuôn kim loại khắc lên giấy xốp.
- **✨ Đổ bóng & Hào quang (Shadow & Glow):** Nổi khối 3D hoặc phát sáng ma mị cho các dòng quote nền tối.
- **📖 Gáy sách 3D, Hạt giấy & Tối viền (Vignette):** Tạo độ cong chiều sâu quang học cho trang sách.

### 4. Typography & Tùy Biến Không Giới Hạn
- Tuyển tập font có chân & không chân hỗ trợ tiếng Việt trọn vẹn: *EB Garamond, Alegreya, STIX Two Text, Lora, Literata, Courier Prime, Be Vietnam Pro, Helvetica*.
- Điều chỉnh thời gian thực: Cỡ chữ, Giãn dòng (*Line-height*), Giãn chữ (*Letter-spacing*), Thụt lề (*Text-indent*).
- Bộ chọn màu tự do cho cả Giấy và Mực (tặng kèm nút màu mực xanh bút máy `#263b72`).
- Nhấn phím `Tab` để thụt đầu dòng tự nhiên không bị nhảy con trỏ.

### 5. Xuất Ảnh Chuẩn In Ấn & Lưu Trữ
- **Xuất ảnh 4K:** Độ nét phóng đại `scale: 4` (~2100px - 2200px), tự động khử răng cưa text.
- **Tự động ghi nhớ (Local Storage):** Toàn bộ font, màu sắc, thanh trượt đều được lưu tự động trên máy, tắt trình duyệt bật lại không bị mất.

---

## 🚀 Hướng Dẫn Sử Dụng Nhanh

### Chạy trực tiếp trên máy (Không cần cài đặt)
1. Tải file `index.html` về máy.
2. Nhấp đúp chuột để mở trực tiếp bằng bất kỳ trình duyệt nào (Chrome, Safari, Edge, Cốc Cốc, Firefox).
3. Bấm chuột vào bất kỳ chữ nào trên trang sách để chỉnh sửa nội dung.
4. Tinh chỉnh hiệu ứng trên thanh công cụ và bấm **`📸 Tải PNG`** để lấy ảnh.

### Bật Web Online Miễn Phí (Qua GitHub Pages)
Nếu muốn dùng trên điện thoại hoặc chia sẻ link cho bạn bè:
1. Đổi tên file HTML của bạn thành `index.html`.
2. Tạo một Repository mới trên GitHub và upload file `index.html` lên.
3. Vào **Settings** của Repo -> Chọn mục **Pages** ở cột bên trái.
4. Ở phần **Branch**, chọn `main` (hoặc `master`) và bấm **Save**.
5. Đợi 1 phút, GitHub sẽ cấp cho bạn một đường link web miễn phí chạy 24/7 dạng:
https://<username>.github.io/<tên-repo>/
---

## 🛠️ Công Nghệ Sử Dụng

- **HTML5 & CSS3:** Thiết kế Responsive, CSS Variables, Flexbox, Typography Grid.
- **SVG Filters:** `feTurbulence`, `feDisplacementMap`, `feGaussianBlur` xử lý biến dạng bề mặt giấy vật lý.
- **JavaScript (ES6):** Xử lý văn bản, DOM Manipulation, LocalStorage API.
- **html2canvas:** Thư viện trích xuất DOM thành Canvas độ phân giải cao.
- **Google Fonts:** Tích hợp bộ font chữ in ấn quốc tế hỗ trợ tiếng Việt.

---

## 📝 Phím Tắt Tiện Lợi

| Phím tắt | Chức năng |
| :--- | :--- |
| `Tab` | Thụt đầu dòng chuẩn sách (`&emsp;&emsp;`) |
| `Ctrl / Cmd + B` | In đậm chữ |
| `Ctrl / Cmd + I` | In nghiêng chữ |
| `Ctrl / Cmd + U` | Gạch chân chữ |

---

## 📄 License
Phát hành dưới giấy phép [MIT License](LICENSE). Thoải mái sử dụng cho mục đích cá nhân, viết lách, sáng tạo nội dung hoặc phát triển thêm tính năng!
