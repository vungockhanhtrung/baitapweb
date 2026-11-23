# Nhật ký sử dụng AI (AI_LOG)
- **Sinh viên thực hiện:** Vũ Ngọc Khánh Trung
- **Mã sinh viên:** 2071020209 – Lớp CNTT 20-04

## 1. Hiện trạng & Vấn đề trước khi hỏi AI
- **Bối cảnh:** Khi thu hẹp màn hình xuống `320px` ở phiên bản V3, các thẻ dự án bị bó hẹp và xuất hiện thanh cuộn ngang khi chứa đường dẫn GitHub dài. Ngoài ra cần chuẩn hóa bộ 4 tệp bàn giao theo yêu cầu Bài 8.
- **Nhận định ban đầu:** Nguyên nhân do Grid mặc định giữ `minmax(auto, 1fr)` khiến cột không chịu co nhỏ hơn nội dung bên trong, và các liên kết không có khoảng trắng không tự ngắt dòng.

## 2. Gợi ý từ công cụ AI
- **Công cụ sử dụng:** Gemini
- **Nội dung hỗ trợ:**
  1. Gợi ý kết hợp `minmax(0, 1fr)` cùng `min-width: 0` trên `.card` và `overflow-wrap: anywhere` cho `.card-link`.
  2. Gợi ý khung mẫu 8 mục cho `README.md` và cấu trúc bảng kiểm thử `evidence-index.md`.

## 3. Quyết định của sinh viên & Lý do
- **Chấp nhận:** Áp dụng `min-width: 0` và `overflow-wrap: anywhere` riêng cho thẻ liên kết (không áp dụng cho toàn bộ `body` để tránh ngắt từ giữa chừng ở các đoạn văn bản thông thường).
- **Tự chỉnh sửa:** Tự tính toán lại 2 mốc breakpoint riêng cho nội dung cá nhân là `640px` và `960px`, tự viết nội dung thông tin sinh viên và tự tạo tệp đồ họa `assets/images/avatar.svg`.

## 4. Kiểm chứng thực tế sau khi sửa
- **Thao tác thử:** Mở Chrome DevTools, đặt kích thước `320x568`, kiểm tra thẻ dự án số 3 chứa link GitHub và chạy lệnh `document.documentElement.scrollWidth > window.innerWidth` trong Console.
- **Kết quả:** Console trả về `false` (hết cuộn ngang), đường dẫn tự xuống dòng gọn gàng trong khung card.