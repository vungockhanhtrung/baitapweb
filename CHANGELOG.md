# Nhật ký thay đổi (CHANGELOG)

## [v8] - 2026-11-23 (Release Note Bàn Giao A3)
### Thay đổi chính
- Hoàn thiện bộ tài liệu bàn giao gồm `README.md`, `CHANGELOG.md`, `AI_LOG.md` và `docs/evidence-index.md`.
- Rà soát toàn bộ đường dẫn tương đối (`css/style.css`, `assets/images/avatar.svg`) đảm bảo phân biệt chữ hoa/thường chính xác trên môi trường Linux của GitHub Pages.
- Gắn nhãn phiên bản `v8` cho commit cuối cùng.
### Đã kiểm tra
- Đối chiếu mã SHA giữa máy cục bộ (Local), kho lưu trữ GitHub (Repo) và bản triển khai (GitHub Pages).
- Kiểm thử chéo toàn bộ liên kết điều hướng và biểu mẫu trên cửa sổ ẩn danh.
### Hạn chế hiện tại
- Form liên hệ chỉ dừng ở mức mô phỏng xác thực HTML5, chưa có backend xử lý lưu trữ.

## [v7] - Triển khai GitHub Pages
- Cấu hình xuất bản từ nhánh `main` thư mục `/ (root)`.
- Sửa lỗi đường dẫn tương đối cho trang kết quả và kiểm tra mã trạng thái HTTP 200 trên tab Network.

## [v5] - Hiệu ứng CSS, Form tĩnh và UX
- Bổ sung trạng thái `:hover`, `:active`, `:focus-visible` cho điều hướng bằng phím `Tab`.
- Tạo form liên hệ có ràng buộc dữ liệu (`required`, `minlength`, `maxlength`) và trang `ket-qua.html`.

## [v4] - Responsive Web Design
- Tái cấu trúc CSS theo hướng Mobile-first (mặc định 1 cột cho màn hình `320px`).
- Bổ sung 2 breakpoint có tính toán: `640px` (2 cột) và `960px` (3 cột).

## [v2 - v3] - Cấu trúc HTML5 Semantic & CSS Layout
- Chuyển đổi khung trang sang thẻ ngữ nghĩa HTML5 (`header`, `nav`, `main`, `section`, `article`, `footer`).
- Thiết lập Box Model (`border-box`), Flexbox cho menu và CSS Grid cho danh sách dự án.