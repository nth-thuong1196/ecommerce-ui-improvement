# AI Usage Log

## 1. Công cụ AI
**Tên công cụ:** Gemini (Google)

## 2. Mục đích sử dụng
- Phân tích nghiệp vụ và UX/UI của website thương mại điện tử thực tế (LocknLock).
- Giải thích phương pháp tiếp cận thiết kế Mobile-First và cách tổ chức layout.
- Đề xuất cấu trúc HTML5 Semantic và hệ thống CSS3 (Grid/Flexbox) cho trang chủ.
- Hỗ trợ tạo khung mã nguồn cơ bản để làm cơ sở phát triển dự án.

## 3. Prompt đã sử dụng
- **Prompt 1:** "Bạn là chuyên gia phân tích nghiệp vụ và thiết kế trải nghiệm người dùng... Tôi đang khảo sát website: LocknLock... Hãy giúp tôi lập bảng phân tích các khu vực: Trang chủ, Danh mục sản phẩm, Chi tiết sản phẩm, Tìm kiếm, Giỏ hàng..."
- **Prompt 2:** "Tôi đang thực hiện bài tập phát triển giao diện website... Tôi muốn cải tiến khu vực: trang chủ... Hãy đề xuất: Bố cục, thành phần HTML, cách tổ chức CSS, cách hiển thị Desktop/Mobile, những điểm cần kiểm tra..."
- **Prompt 3:** "Dựa trên phương án đã thống nhất, hãy tạo một trang giao diện thương mại điện tử bằng HTML5 và CSS3..."

## 4. Kết quả AI đề xuất
- Cung cấp bảng phân tích chi tiết ưu/nhược điểm giao diện hiện tại của LocknLock kèm đề xuất cải tiến (AJAX filter, Typo tolerance trong tìm kiếm).
- Đề xuất chiến lược cấu trúc file rõ ràng (Block Element Modifier - BEM cơ bản, tách riêng HTML và CSS).
- Tạo mã nguồn HTML5 semantic (dùng `<header>`, `<article>`, `<figure>`) và CSS3 sử dụng CSS Variables, Flexbox cho Header/Card và Grid cho Product List.
- Tích hợp Media Queries để xử lý Responsive.

## 5. Kiểm tra và điều chỉnh
- **Đã kiểm tra:** Khả năng co giãn của giao diện khi chuyển đổi từ Desktop (màn hình rộng, 4 cột sản phẩm) sang Mobile (màn hình hẹp, 2 cột sản phẩm).
- **Đã kiểm tra:** Các thuộc tính hiển thị văn bản như `-webkit-line-clamp` hoạt động chính xác khi tên sản phẩm quá dài.
- **Đã kiểm tra:** Tỷ lệ khung hình `aspect-ratio` giúp ảnh không bị méo.
- **Điều chỉnh:** Tự cập nhật lại các tham số hình ảnh placeholder, màu sắc thương hiệu (brand colors) và font chữ theo sở thích thiết kế cá nhân.

## 6. Phần tôi hiểu và có thể giải thích
- **CSS Grid & Flexbox:** Tôi có thể giải thích cách thuộc tính `display: grid; grid-template-columns: repeat(4, 1fr);` chia đều 4 cột trên desktop và cách `display: flex;` được sử dụng để căn chỉnh logo, ô tìm kiếm, giỏ hàng trong Header.
- **Media Queries:** Cách sử dụng `@media (min-width: 768px)` để ghi đè (override) CSS dành riêng cho thiết bị lớn theo phương pháp Mobile-First.
- **Semantic HTML:** Tại sao dùng `<article>` cho thẻ sản phẩm lại tốt hơn dùng `<div>` (tốt cho SEO và khả năng tiếp cận - Accessibility).
- **CSS Variables:** Hiểu cách khai báo `:root { --primary-color: #... }` giúp thay đổi màu chủ đạo của toàn website nhanh chóng chỉ bằng một dòng code.