# Trợ lý Tóm Tắt Web (Gemini) - Giao diện Bảng

[![Powered by](https://img.shields.io/badge/Powered%20by-Gemini%20API-blueviolet)](https://ai.google.dev/)

Một kịch bản Tampermonkey mạnh mẽ, biến trình duyệt của bạn thành một công cụ phân tích thông minh. Nhấn **`Alt + Q`** để tóm tắt bất kỳ trang web nào và nhận lại kết quả dưới dạng một bảng phân tích hiện đại, rõ ràng, giúp bạn nắm bắt thông tin nhanh chóng và hiệu quả hơn bao giờ hết.

---

## 🖼️ Xem trước Giao diện

Trải nghiệm một giao diện đọc hoàn toàn mới, được thiết kế để tối ưu hóa sự tập trung và khả năng tiếp thu thông tin.

*Giao diện chính khi tóm tắt một bài viết về lập trình:*
![Giao diện xem trước]([https://i.imgur.com/gH8oA13.png](https://i.ibb.co/dJ6WsLTF/image.png))
<a href="https://ibb.co/Kz70cLPd"><img src="https://i.ibb.co/Kz70cLPd/image.png" alt="image" border="0"></a>
---

## ✨ Tính năng Nổi bật

* **⚡ Tóm tắt Tức thì**: Kích hoạt chỉ bằng một phím tắt duy nhất (`Alt + Q`). Không cần sao chép, không cần dán link vào một trang web khác.
* **📊 Giao diện Bảng Thông minh**: Nội dung được AI phân tích và trình bày khoa học dưới dạng bảng với 3 cột:
    * `#`: Số thứ tự các ý chính.
    * `Ý Chính`: Câu chủ đề hoặc luận điểm cốt lõi.
    * `Chi Tiết & Phân Tích`: Các luận cứ, diễn giải, và dữ liệu hỗ trợ, được trình bày dưới dạng danh sách dễ đọc.
* **🔑 Tự động In đậm Từ khóa**: AI tự động xác định và **in đậm** các từ khóa (keywords) hoặc cụm từ quan trọng nhất trong phần chi tiết, giúp bạn tập trung vào những điểm cốt lõi.
* **💬 Phân tích Cả Bình luận**: Kịch bản không chỉ tóm tắt nội dung chính mà còn tự động tìm, trích xuất và phân tích cả phần bình luận (comments section), cung cấp cho bạn một cái nhìn đa chiều về chủ đề.
* **🎨 Giao diện Hiện đại & Đẹp mắt**:
    * Lớp phủ (overlay) với hiệu ứng `backdrop-filter: blur(8px)` sang trọng.
    * Loader 3D xoay ấn tượng trong lúc chờ xử lý.
    * Hộp thoại kết quả được thiết kế với màu sắc và font chữ dễ đọc, tối ưu cho việc đọc lâu.
* **📋 Sao chép Dễ dàng**: Nút "Sao chép" cho phép bạn lấy toàn bộ nội dung tóm tắt dưới dạng văn bản có cấu trúc để dễ dàng lưu trữ hoặc chia sẻ.
* **📝 Hỗ trợ Markdown**: Hiển thị chính xác các định dạng Markdown cơ bản như `<strong>` (in đậm), `<em>` (in nghiêng), và đặc biệt là `<code>` cho các đoạn mã, công thức, giúp giữ nguyên ngữ cảnh kỹ thuật.
* **🧠 Tùy biến Prompt**: Dễ dàng thay đổi "câu lệnh yêu cầu" (`prompt`) gửi đến Gemini API trực tiếp trong mã nguồn để điều chỉnh văn phong, độ sâu, hoặc cấu trúc của bản tóm tắt theo ý muốn cá nhân.

---

## 🚀 Cài đặt và Cấu hình (3 Bước)

Để kịch bản hoạt động, bạn cần thực hiện 3 bước đơn giản sau:

### Bước 1: Cài đặt Tiện ích Tampermonkey

Nếu bạn chưa có, hãy cài đặt tiện ích mở rộng **Tampermonkey** cho trình duyệt của mình. Đây là nền tảng cần thiết để chạy các userscript.

* [Dành cho **Chrome**](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
* [Dành cho **Firefox**](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/)
* [Dành cho **Edge**](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpaadaobahmlepeloendndfphd)
* [Dành cho **Safari**](https://www.tampermonkey.net/?browser=safari)

### Bước 2: Cài đặt Kịch bản "Trợ lý Tóm Tắt Web"

1.  **Nhấp vào liên kết cài đặt dưới đây:**
    * [**Cài đặt Kịch bản Ngay**](https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO/main/script.user.js) 2.  Tampermonkey sẽ tự động mở một tab mới hiển thị mã nguồn của kịch bản.
3.  Nhấp vào nút **`Install`** để hoàn tất cài đặt.

### Bước 3: Cấu hình Gemini API Key (Bắt buộc)

Đây là bước quan trọng nhất để kích hoạt trí tuệ nhân tạo.

1.  **Lấy API Key của bạn từ Google AI Studio:**
    * Truy cập [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey).
    * Đăng nhập bằng tài khoản Google của bạn.
    * Nhấp vào nút "**Create API key in new project**".
    * Một chuỗi ký tự bí mật sẽ hiện ra. Hãy **sao chép** (copy) chuỗi API key này.

2.  **Dán API Key vào kịch bản:**
    * Mở **`Dashboard`** (Bảng điều khiển) của Tampermonkey từ thanh công cụ của trình duyệt.
    * Trong danh sách các kịch bản đã cài, tìm `Trợ lý Tóm Tắt Web (Gemini) - Giao diện Bảng` và nhấp vào biểu tượng **`Edit`** (</>).
    * Tìm đến dòng số `15` trong trình soạn thảo mã:

      ```javascript
      // DÒNG 15
      const API_KEY = 'YOUR_GEMINI_API_KEY';
      ```

    * **Xóa** `'YOUR_GEMINI_API_KEY'` và **dán** API key bạn vừa sao chép vào giữa hai dấu nháy đơn. Nó sẽ trông giống như thế này:

      ```javascript
      // VÍ DỤ SAU KHI DÁN
      const API_KEY = 'AIzaSy...AbCdEfGhIjKlMnOpQrStU';
      ```

    * Lưu lại kịch bản bằng cách nhấn `Ctrl + S` hoặc vào menu `File` -> `Save`.

**Hoàn tất!** Bây giờ bạn có thể truy cập bất kỳ trang web bài viết nào và nhấn **`Alt + Q`** để xem phép màu xảy ra.

---

## 🔧 Tùy chỉnh Prompt (Dành cho người dùng nâng cao)

Bạn muốn AI tóm tắt theo một phong cách khác? Ví dụ: theo kiểu 5 dòng cho người bận rộn, hoặc tập trung phân tích ưu nhược điểm? Rất đơn giản!

1.  Mở trình chỉnh sửa kịch bản trong Tampermonkey.
2.  Tìm đến hàm `startSummarization()`, khoảng dòng `300`.
3.  Chỉnh sửa nội dung văn bản bên trong biến `prompt`. Đây chính là "bộ não" chỉ dẫn cho AI biết phải làm gì.

    ```javascript
    const prompt = `Bạn là một chuyên gia phân tích và tóm tắt nội dung.
    Nhiệm vụ: Đọc và tóm tắt văn bản dưới đây, bao gồm cả nội dung chính và phần bình luận.
    Yêu cầu định dạng đầu ra:
    1.  Chia nội dung tóm tắt thành các ý chính riêng biệt.
    2.  Mỗi ý chính PHẢI bắt đầu bằng một dòng có cú pháp Markdown heading 2, ví dụ: "## Tiêu đề của ý chính".
    // ... (Bạn có thể thêm, xóa, hoặc sửa các yêu cầu tại đây) ...
    5.  QUAN TRỌNG NHẤT: Trong phần chi tiết, hãy xác định và **in đậm** các từ khóa (keywords) hoặc cụm từ quan trọng nhất...
    ---
    NỘI DUNG CẦN TÓM TẮT:
    ${pageText}`;
    ```

---

## 🤝 Đóng góp

Mọi sự đóng góp đều được chào đón! Nếu bạn có ý tưởng để cải thiện kịch bản, vui lòng tạo một [Issue](https://github.com/YOUR_USERNAME/YOUR_REPO/issues) để thảo luận hoặc tạo một [Pull Request](https://github.com/YOUR_USERNAME/YOUR_REPO/pulls) với những thay đổi của bạn.

---

## 📄 Giấy phép

Dự án này được cấp phép theo [Giấy phép MIT](./LICENSE).
