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

## CHO BUỔI 2

## 7. Các nội dung AI hỗ trợ bổ sung trong quá trình phát triển

- **CSS Selectors và Box Model:** Hướng dẫn sử dụng Element Selector, Class Selector và Descendant Selector để định dạng các thành phần sản phẩm. Giải thích cách hoạt động của `margin`, `padding`, `border`, `border-radius` và `box-sizing`.
- **Flexbox:** Hỗ trợ hoàn thiện thanh menu điều hướng bằng `display: flex`, `justify-content`, `align-items`, `gap` và `flex-wrap` nhằm căn chỉnh các liên kết menu ở vị trí trung tâm.
- **CSS Grid:** Giải thích cách tổ chức danh sách sản phẩm bằng `grid-template-columns`, `repeat()`, `fr` và `gap`; hướng dẫn điều chỉnh số cột hiển thị giữa Mobile và Desktop.
- **Hiệu ứng tương tác:** Hướng dẫn bổ sung trạng thái `:hover` và `:focus-visible` cho các liên kết menu, giúp giao diện trực quan hơn và hỗ trợ người dùng điều hướng bằng bàn phím.

## 8. Prompt đã sử dụng bổ sung

- **Prompt 4:** "Tôi muốn tìm hiểu và thực hành CSS Selectors và Box Model trên website hiện tại. Hãy hướng dẫn cách sử dụng Element Selector, Class Selector, Descendant Selector, margin, padding, border và border-radius mà không làm thay đổi cấu trúc HTML."
- **Prompt 5:** "Tôi muốn thực hành Flexbox trên thanh menu điều hướng hiện tại. Hãy giải thích cách sử dụng display, justify-content, align-items, gap và flex-wrap để căn chỉnh các liên kết menu vào giữa."
- **Prompt 6:** "Hãy giải thích cách sử dụng CSS Grid để bố trí danh sách sản phẩm, điều chỉnh số cột, khoảng cách giữa các sản phẩm và cách sử dụng object-fit: cover để hình ảnh không bị méo."
- **Prompt 7:** "Tôi muốn bổ sung hiệu ứng hover và focus cho các liên kết trong website. Hãy hướng dẫn sử dụng transition, :hover và :focus-visible, đảm bảo màu chữ và màu nền dễ nhìn, không làm thay đổi bố cục quá nhiều."

## 9. Kết quả AI đề xuất bổ sung

- Đưa ra các đoạn CSS có thể bổ sung hoặc chỉnh sửa trực tiếp trong file `style.css` hiện tại.
- Hướng dẫn xác định đúng selector cần chỉnh sửa, hạn chế tạo các khối CSS trùng lặp.
- Đề xuất sử dụng Flexbox để căn giữa các liên kết trong thanh menu.
- Giải thích cách sử dụng `repeat(2, 1fr)` và `repeat(4, 1fr)` để phân chia các cột sản phẩm có kích thước bằng nhau.
- Bổ sung hiệu ứng chuyển màu, đổi màu nền và dịch chuyển nhẹ khi di chuột qua liên kết.
- Bổ sung đường viền `outline` cho trạng thái `:focus-visible` nhằm cải thiện khả năng tiếp cận.

## 10. Kiểm tra và điều chỉnh bổ sung

- **Đã thực hành:** Chỉnh sửa CSS cho thanh menu điều hướng và sử dụng Flexbox để căn giữa các liên kết.
- **Đã thực hành:** Điều chỉnh số cột của danh sách sản phẩm bằng CSS Grid và tìm hiểu sự khác nhau giữa các đơn vị `fr`.
- **Đã thực hành:** Bổ sung các trạng thái tương tác `:hover` và `:focus-visible` cho liên kết menu.
- **Đã điều chỉnh:** Rà soát lại các selector CSS hiện có để chỉnh sửa trực tiếp thay vì tạo thêm những khối CSS trùng lặp.
- **Đã tìm hiểu:** Cách kiểm tra hiệu ứng bằng chuột và phím `Tab` trên trình duyệt.

## 11. Phần kiến thức bổ sung tôi hiểu và có thể giải thích

- **CSS Selectors:** Phân biệt được cách lựa chọn phần tử HTML bằng tên thẻ, tên class và quan hệ phần tử cha - con.
- **Box Model:** Hiểu sự khác nhau giữa khoảng cách bên ngoài (`margin`), khoảng cách bên trong (`padding`) và đường viền (`border`).
- **Flexbox:** Hiểu vai trò của phần tử cha trong việc điều khiển vị trí các phần tử con, đặc biệt là cách căn giữa bằng `justify-content: center`.
- **CSS Grid:** Hiểu cách chia bố cục thành các cột bằng `grid-template-columns` và cách sử dụng `fr` để phân chia không gian.
- **Hover và Focus:** Phân biệt trạng thái khi người dùng di chuột (`:hover`) và khi điều hướng bằng bàn phím (`:focus-visible`).
- **Transition:** Hiểu cách sử dụng `transition` để tạo hiệu ứng chuyển đổi mượt mà giữa các trạng thái CSS.