# Report 1 Page – FIT4012 Lab 2

**Họ và tên:** Phạm Hoàng Hải 
**Mã sinh viên:** 1871020214


## 1. Mục tiêu
Hoàn thành việc triển khai và kiểm thử hai thuật toán mã hóa cổ điển: Caesar Cipher và Rail Fence Cipher trên ngôn ngữ C++.

## 2. Cách làm
- Hoàn thiện Caesar Cipher cho chữ thường, dấu cách và giải mã.
- Hoàn thiện Rail Fence Cipher cho giải mã, giữ dấu cách, kiểm tra đầu vào và đọc file.
- Chạy thử trên nhiều test case thực tế (I LOVE YOU, hello world...).

## 3. Kết quả chính
### 3.1 Caesar Cipher
| Input | Key | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 3 | L ORYH BRX | Mã hóa đúng, giữ nguyên dấu cách. |
| hello world | 5 | mjqqt btwqi | Xử lý tốt chữ thường. |
| L ORYH BRX | 3 | I LOVE YOU | Giải mã chính xác về bản gốc. |

### 3.2 Rail Fence Cipher
| Input | Rails | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 2 | ILV O OEYU | Hoán vị ziczac 2 hàng chuẩn. |
| I LOVE YOU | 4 | I  EYLVOOU | Kết quả 4 hàng khớp với thực tế chạy máy. |
| ILV O OEYU | 2 | I LOVE YOU | Giải mã ngược lại thành công. |

### 3.3 Input validation / file input
- Trường hợp đầu vào không hợp lệ: Chương trình hiện thông báo lỗi "Invalid input" khi nhập ký tự không phải chữ cái.
- Kết quả đọc từ `data/input.txt`: Đã test chức năng đọc file (Choice 3) và mã hóa thành công.

## 4. Kết luận
Em đã hiểu rõ cách vận hành của mã hóa thay thế và hoán vị. Khó khăn lớn nhất là xử lý ma trận cho Rail Fence nhưng đã giải quyết được nhờ việc vẽ sơ đồ đường đi. Bài lab giúp em thành thạo hơn trong việc thao tác chuỗi và quản lý file.
