
---
## I. A.I (Thông số cấu hình)
*   **Nền tảng:** Google AI Studio
*   **Chế độ (Mode):** Code, reasoning and chat
*   **Thông số kỹ thuật:**
    *   `Temperature`: 0.8
    *   `Media resolution`: Medium
    *   `Thinking level`: High
    *   `Top p`: 0.8

---

## II. LỆNH DÙNG (INPUT)

**1. Thiết lập vai trò và cung cấp mã nguồn gốc:**
> "Trong đoạn chat này, bạn là 1 lập trình viên full stack có nhiều năm kinh nghiệm, tôi là sinh viên sắp tốt nghiệp, nhiệm vụ của bạn là hướng dẫn, giải đáp những thắc mắc và bổ sung, sửa đổi những lỗi tôi mắc phải trong những gì tôi cung cấp cho bạn phù hợp với những yêu cầu trong bài tập của tôi. Trước tiên, hãy nhìn vào đoạn code HTML sau, chỉ nhìn đoạn code và chưa làm gì: [Mã nguồn HTML gốc]"

**2. Yêu cầu khớp giao diện theo hình ảnh:**
> "Ok giờ từ đoạn code đó, giúp tôi thêm những thứ cần thiết khác miễn sao giống với bức ảnh này nhất có thể, chú ý: không làm thay đổi nội dung trong <body> của đoạn mã mà em cung cấp."

**3. Yêu cầu mở rộng không gian:**
> "Tháo khung giới hạn của đoạn mã mà thầy đã cung cấp."

**4. Yêu cầu tối ưu hóa cấu trúc (Kích hoạt Code Execution):**
> "Giờ hãy tối ưu lại chính code của thầy vừa hướng dẫn một cách hợp lý nhất để dễ phát triển thêm những tính khác sau này. Không làm thay đổi <body>."

**5. Yêu cầu tinh chỉnh hiển thị:**
> "Ở phần nội dung bên phải, không cần phải đổi màu vùng đang được chọn."

---

## III. KẾT QUẢ (OUTPUT)

```html
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <title>Học trực tuyến CNTT</title>
    <style>
        /* 1. KHAI BÁO BIẾN */
        :root {
            --bg-sidebar: #eeeeee;
            --bg-active-sidebar: #7b7b7b; /* Chỉ dùng cho menu bên trái */
            --text-main: #000000;
            --text-white: #ffffff;
            --font-main: "Times New Roman", Times, serif;
        }
        

        /* 2. RESET & CẤU HÌNH CHUNG */
        html, body {
            margin: 0;
            padding: 0;
            height: 100%;
            font-family: var(--font-main);
        }

        table {
            border-collapse: collapse;
            width: 100%;
            height: 100vh;
            border: none;
        }

        /* 3. CỘT BÊN TRÁI (SIDEBAR) */
        td[width="20%"] {
            background-color: var(--bg-sidebar);
            vertical-align: top;
            padding: 0;
            border-right: 1px solid #ddd;
        }

        /* Định dạng menu bên trái */
        td[width="20%"] ul {
            list-style-type: none;
            padding: 0;
            margin: 0;
        }

        /* CHỈ ĐỔI MÀU VÙNG CHỌN CHO MENU BÊN TRÁI */
        td[width="20%"] li:first-child {
            background-color: var(--bg-active-sidebar);
        }

        td[width="20%"] li:first-child a {
            color: var(--text-white);
        }

        td[width="20%"] a {
            text-decoration: none;
            color: var(--text-main);
            display: block;
            padding: 12px 20px;
            font-size: 1.1rem;
        }

        /* 4. CỘT BÊN PHẢI (NỘI DUNG CHÍNH) */
        td[width="80%"] {
            vertical-align: top;
            padding: 40px 60px;
            background-color: white;
        }

        /* Giữ danh sách bên phải nguyên bản, không bị ảnh hưởng bởi CSS vùng chọn */
        td[width="80%"] ol {
            margin-top: 15px;
            line-height: 2;
            font-size: 1.1rem;
        }

        td[width="80%"] li {
            background-color: transparent; /* Đảm bảo không có màu nền */
            color: var(--text-main);       /* Đảm bảo chữ luôn màu đen */
        }

        /* 5. TIÊU ĐỀ */
        h1 {
            margin-top: 0;
            font-size: 2.2rem;
        }

        h2 {
            margin-top: 30px;
            font-size: 1.5rem;
        }

        /* 6. RESPONSIVE */
        @media (max-width: 768px) {
            table, tr, td {
                display: block !important;
                width: 100% !important;
                height: auto !important;
            }
        }
    </style>
</head>
<body>
    <table border="0" width="100%">
        <td width="20%">
            <ul>
                <li><a>Trang chủ</a></li>
                <li><a>Khóa học</a></li>
                <li><a>Diễn đàn</a></li>
                <li><a>Liên hệ</a></li>
            </ul>
        </td>

        <td width="80%">
            <h1>Học trực tuyến Công nghệ thông tin</h1>
            <h2>Các khóa học:</h2>
            <ol>
                <li>Lập trình cơ bản</li>
                <li>Cấu trúc dữ liệu</li>
                <li>Thiết kế web</li>
            </ol>
        </td>
    </table>
</body>
</html>
```

---

Hy vọng file README này sẽ giúp ích cho em trong việc nộp bài hoặc lưu trữ dự án. Chúc em có một kỳ tốt nghiệp thật thành công!
