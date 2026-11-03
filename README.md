# E-commerce UI Improvement

## 1. Giới thiệu
Dự án này là bài tập thực hành phát triển giao diện Front-end, tập trung vào việc tái thiết kế và cải thiện trải nghiệm người dùng (UX/UI) cho khu vực Trang chủ của một website thương mại điện tử. Mục tiêu chính là áp dụng thiết kế Mobile-First, tối ưu hóa không gian hiển thị và tăng cường sự tiện lợi cho khách hàng khi mua sắm trực tuyến.

## 2. Website tham khảo
- **Tên website:** LocknLock Việt Nam
- **URL:** https://www.locknlock.vn/
- **Khu vực đã khảo sát:** Trang chủ (Header, Hero Banner, Danh sách sản phẩm nổi bật).

## 3. Chức năng
- Hiển thị danh sách sản phẩm theo dạng lưới (Grid).
- Hiển thị đầy đủ thông tin cốt lõi của sản phẩm: Hình ảnh, Nhãn giảm giá, Tên, Giá bán, Giá gốc và Nút thao tác ("Thêm vào giỏ").
- Bố cục linh hoạt (Responsive), tự động điều chỉnh tối ưu cho cả màn hình máy tính (Desktop) và điện thoại (Mobile).

## 4. Công nghệ
- HTML5 (Sử dụng Semantic tags: `<header>`, `<main>`, `<section>`, `<article>`, `<figure>`)
- CSS3 (Sử dụng CSS Variables, Flexbox, Grid Layout, Media Queries, CSS Transitions)

## 5. Cách chạy
Dự án không yêu cầu cài đặt máy chủ (Backend) hay Node.js. 
Chỉ cần giải nén thư mục dự án và mở file `index.html` bằng bất kỳ trình duyệt web nào (Google Chrome, Safari, Edge, Firefox...).

## 6. Cải tiến đã thực hiện
- **Vấn đề ban đầu (từ website tham khảo):** Việc tải nhiều hình ảnh/video nặng làm chậm tốc độ trang trên mobile; layout mô tả sản phẩm dạng ảnh dài (long-image) gây khó đọc; thanh tìm kiếm và giỏ hàng chưa tối ưu không gian hiển thị trên màn hình hẹp.
- **Thay đổi đã thực hiện:** 
  - Áp dụng nguyên tắc **Mobile-First**, cấu trúc lại Header gọn gàng hơn (gom thanh tìm kiếm xuống hàng riêng trên mobile).
  - Chuẩn hóa tỷ lệ hình ảnh sản phẩm (`aspect-ratio: 1/1`) để lưới (grid) luôn đồng đều, không xô lệch dù kích thước ảnh gốc khác nhau.
  - Sử dụng CSS `-webkit-line-clamp` để giới hạn độ dài tên sản phẩm (tối đa 2 dòng), giữ cho thẻ sản phẩm luôn gọn gàng.
  - Mở rộng vùng chạm (Touch targets) cho nút "Thêm vào giỏ" trên mobile (tối thiểu 44px) để tránh bấm nhầm.

## 7. Hỗ trợ từ AI
- **Phần AI hỗ trợ:** Khảo sát và phân tích ưu/nhược điểm UX/UI của website gốc; đề xuất chiến lược layout (Grid/Flexbox) và cấu trúc HTML5 ngữ nghĩa; viết khung mã nguồn HTML/CSS cơ sở.
- **Phần tôi thực hiện:** Đặt yêu cầu, kiểm tra cách mã nguồn hoạt động trên trình duyệt, co giãn kích thước cửa sổ để test tính năng Responsive, kiểm tra các hiệu ứng Hover/Click và tổ chức lại dự án.