# Portfolio Cá Nhân – Vũ Ngọc Khánh Trung (A3)

## 1. Sản phẩm này là gì?
Website Portfolio tĩnh giới thiệu thông tin cá nhân, kỹ năng nền tảng và các sản phẩm thực hành của sinh viên **Vũ Ngọc Khánh Trung** (MSV: `2071020209`, Lớp `CNTT 20-04` – Khoa Công nghệ Thông tin, Đại học Đại Nam) trong học phần **Thiết kế Web và Triển khai hệ thống phần mềm (FIT4014)**.

## 2. Demo trực tuyến
- **URL GitHub Pages:** `https://<username-cua-ban>.github.io/a3-portfolio-trung/`
- **Nhánh xuất bản:** `main` – Thư mục `/ (root)`

## 3. Tính năng hiện có
- **Giới thiệu bản thân:** Hiển thị thông tin sinh viên, định hướng học tập và ảnh đại diện vector sắc nét.
- **Kỹ năng & Dự án:** Trình bày theo thẻ (Card) dạng lưới tự thích nghi từ 1 cột (điện thoại) lên 2–3 cột (máy tính).
- **Điều hướng mượt & Hỗ trợ bàn phím:** Menu dính đầu trang (`sticky`), hỗ trợ nhảy neo nội bộ và hiển thị viền focus (`:focus-visible`) rõ ràng khi bấm phím `Tab`.
- **Biểu mẫu liên hệ có kiểm tra dữ liệu:** Ràng buộc nhập liệu chuẩn HTML5 (`required`, `email`, `minlength`) và chuyển hướng sang trang xác nhận `ket-qua.html`.

## 4. Cách mở hoặc chạy thử
1. **Xem trực tiếp:** Truy cập URL GitHub Pages ở Mục 2 bằng trình duyệt bất kỳ (khuyến nghị mở bằng cửa sổ ẩn danh để kiểm tra quyền truy cập công khai).
2. **Chạy trên máy cục bộ (Local):**
   - Tải hoặc clone repository về máy.
   - Mở thư mục `a3-portfolio-trung` bằng Visual Studio Code.
   - Nhấp đúp vào tệp `index.html` hoặc chạy qua tiện ích Live Server.

## 5. Cấu trúc thư mục
```text
a3-portfolio-trung/
├── index.html              # Trang chủ nội dung chính
├── ket-qua.html            # Trang mô phỏng kết quả gửi form
├── README.md               # Tài liệu hướng dẫn dự án
├── CHANGELOG.md            # Nhật ký thay đổi các phiên bản
├── AI_LOG.md               # Nhật ký sử dụng AI có trách nhiệm
├── css/
│   └── style.css           # Định kiểu giao diện & Responsive
├── assets/
│   └── images/
│       └── avatar.svg      # Hình ảnh minh họa đại diện
└── docs/
    └── evidence-index.md   # Bảng tổng hợp minh chứng kiểm thử
```

## 6. Đã kiểm tra
- Kiểm tra cấu trúc HTML5 Semantic (đúng 1 thẻ `<h1>`, 1 thẻ `<main>`, đầy đủ `alt` cho hình ảnh) qua Chrome DevTools Elements.
- Kiểm tra hiển thị Responsive tại các mốc `320px`, `639px`, `640px`, `959px`, `960px` và `1440px` (không xuất hiện thanh cuộn ngang).
- Kiểm tra 3 kịch bản nhập biểu mẫu: bỏ trống, nhập sai định dạng email/độ dài, và nhập hợp lệ chuyển sang `ket-qua.html`.
- Kiểm tra trạng thái HTTP `200` cho toàn bộ tài nguyên CSS/SVG trên tab Network của GitHub Pages.

## 7. Giới hạn / Chưa kiểm tra
- Biểu mẫu liên hệ là form tĩnh phía client (`method="get"`), **chưa gửi email thật và chưa lưu dữ liệu vào cơ sở dữ liệu**.
- Chưa kiểm thử hiển thị thực tế trên các thiết bị iOS/Android vật lý đời cũ (mới kiểm thử qua giả lập thiết bị của Chrome DevTools).

## 8. Nguồn tài nguyên và Khai báo AI
- Hình ảnh `avatar.svg` được tự thiết kế bằng mã SVG thuần.
- Có sử dụng công cụ AI hỗ trợ gợi ý cấu trúc bố cục CSS Grid và rà soát tài liệu bàn giao; toàn bộ mã nguồn đã được sinh viên tự kiểm thử, chỉnh sửa và xác minh (chi tiết xem tại `AI_LOG.md`).