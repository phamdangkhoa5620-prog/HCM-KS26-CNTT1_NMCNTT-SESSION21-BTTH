## PHẦN 1 – GOOGLING ĐÚNG CÁCH

### 1\. Vì sao câu hỏi văn nói tìm kiếm kém hiệu quả?

* Câu hỏi dài, thiếu từ khóa kỹ thuật.
* Không có thông báo lỗi nguyên văn.
* Google khó xác định chính xác vấn đề cần tìm.

### 2\. Bóc tách lỗi theo 3 thành phần

* **Phần mềm / Hệ điều hành:** Node.js / Windows 11.
* **Mã lỗi:** `npm is not recognized as an internal or external command`.
* **Thao tác:** Nhập lệnh `npm -v` trong Terminal VS Code.

### 3\. Ba câu truy vấn Google

* **Toán tử `site:`**

```text
  site:stackoverflow.com npm not recognized Windows 11 PATH
  ```

* **Toán tử ngoặc kép `" "`**

```text
  "npm is not recognized as an internal or external command"
  ```

* **Toán tử `-`**

```text
  npm not recognized Windows PATH -WindowsXP
  ```

## PHẦN 2 – THẨM ĐỊNH STACKOVERFLOW

### 1\. So sánh hai câu trả lời

|Tiêu chí|Câu trả lời A|Câu trả lời B|
|-|-|-|
|Vote \& tích xanh|+186, có tích xanh|+2, không tích xanh|
|Thời gian|2 năm trước|9 năm trước|
|Tags|Node.js, Windows, npm|Node.js, Windows XP|

### 2\. Kết luận

* Chọn **câu trả lời A** vì có nhiều lượt bình chọn, được chấp nhận và phù hợp Windows.
* Câu trả lời B là bẫy vì hướng dẫn cài driver mạng Windows XP, không liên quan đến lỗi PATH.

### 3\. Quy trình 30 giây đọc lướt

1. Xem tiêu đề câu hỏi.
2. Kiểm tra Tags.
3. Tìm câu trả lời có tích xanh.
4. Kiểm tra số Upvote.
5. Xem thời gian đăng và nội dung hướng dẫn.

## PHẦN 3 – HỎI AI VÀ NHẬN DIỆN RỦI RO

### 1\. Prompt 3 thành phần

**\[CONTEXT – NGỮ CẢNH]**

Tôi vừa cài Node.js trên laptop Windows 11, sử dụng Terminal trong VS Code. Đã thêm đường dẫn Node.js vào PATH và mở Terminal mới nhưng lỗi vẫn còn.

**\[RAW ERROR – LỖI NGUYÊN VĂN]**

```text
'npm' is not recognized as an internal or external command,
operable program or batch file.
```

**\[INSTRUCTION – YÊU CẦU]**

Hãy giải thích nguyên nhân bằng tiếng Việt dễ hiểu và hướng dẫn kiểm tra, khắc phục từng bước an toàn. Không đề xuất lệnh xóa dữ liệu hệ thống.

### 2\. Đánh giá câu trả lời AI

**Không an toàn – Tuyệt đối không chạy lệnh.**

* Lệnh `del /f /s /q C:\\Windows\\System32\\\*` có thể xóa các tệp hệ thống quan trọng.
* Có nguy cơ làm Windows bị lỗi hoặc không thể khởi động.
* Lệnh không liên quan đến việc sửa PATH.

### 3\. Phản hồi lại AI

```text
Lệnh bạn đề xuất có thể xóa các tệp quan trọng
trong Windows System32. Hãy giải thích vì sao lệnh
này liên quan đến lỗi npm PATH.

Vui lòng đưa ra cách kiểm tra PATH an toàn,
không xóa dữ liệu và không ảnh hưởng hệ điều hành.
```

## PHẦN 4 – VIẾT BUG REPORT CHUẨN

### 1\. Tin nhắn kém

```text
Thầy ơi máy em bị lỗi npm rồi,
thầy giúp em với ạ!
```

### 2\. Tin nhắn chuẩn theo Bug Reporting Framework

**Context:** Em vừa cài Node.js trên laptop Windows 11 và sử dụng Terminal trong VS Code.

**Expected:** Khi nhập `npm -v`, Terminal hiển thị phiên bản npm.

**Actual:** Terminal báo lỗi:

```text
'npm' is not recognized as an internal or external command,
operable program or batch file.
```

Em đã thêm PATH và mở Terminal mới nhưng lỗi vẫn còn.

**Log \& Screenshot:** Em gửi ảnh chụp màn hình thông báo lỗi để thầy kiểm tra và hỗ trợ.

### 3\. Phím tắt và lưu ý bảo mật

* **Phím tắt:** `Windows + Shift + S`.
* **Lưu ý:** Che mật khẩu, API Key và thông tin cá nhân trước khi gửi ảnh.

