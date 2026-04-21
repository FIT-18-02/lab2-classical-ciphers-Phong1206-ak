# Report 1 Page – FIT4012 Lab 2

## 1. Mục tiêu
Mục tiêu của bài lab là hiểu và cài đặt hai thuật toán mã hóa cổ điển là Caesar Cipher và Rail Fence Cipher, bao gồm cả mã hóa và giải mã. Đồng thời, thực hành xử lý chuỗi, kiểm tra dữ liệu đầu vào và đọc dữ liệu từ file.

## 2. Cách làm
- Hoàn thiện Caesar Cipher cho chữ thường, dấu cách và giải mã.
- Hoàn thiện Rail Fence Cipher cho giải mã, giữ dấu cách, kiểm tra đầu vào và đọc file.
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Caesar Cipher
| Input | Key | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 3 | L ORYH BRX | Mã hóa đúng, giữ khoảng trắng |
| hello world | 5 | mjqqt btwqi | Xử lý đúng chữ thường |
| LORYH BRX | 3 | I LOVE YOU | Giải mã chính xác |

### 3.2 Rail Fence Cipher
| Input | Rails | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 2 | IOEOLVYU | Mã hóa đúng theo zigzag |
| I LOVE YOU | 4 | IYOOELVU | Rail nhiều hơn -> phân bố khác |
| IOEOLVYU | 2 | ILOVEYOU | Giải mã chính xác |

### 3.3 Input validation / file input
- Trường hợp đầu vào không hợp lệ:
Key âm hoặc bằng 0 → báo lỗi.
Rail < 2 → không hợp lệ.
Chuỗi rỗng → không xử lý.
- Kết quả đọc từ `data/input.txt`:
Đọc file thành công, xử lý từng dòng và áp dụng mã hóa/giải mã đúng yêu cầu.
## 4. Kết luận
Nêu ngắn gọn em học được gì từ bài lab, khó khăn lớn nhất là gì, và điều gì giúp em hiểu rõ hơn về Caesar hoặc Rail Fence Cipher.
Qua bài lab, em hiểu rõ hơn cách hoạt động của các thuật toán mã hóa cổ điển như Caesar Cipher (dịch ký tự theo khóa) và Rail Fence Cipher (sắp xếp theo dạng zigzag). Khó khăn lớn nhất là phần giải mã Rail Fence do phải xác định lại vị trí ký tự ban đầu. Việc làm bài giúp em nắm rõ hơn cách xử lý chuỗi và tư duy thuật toán trong lập trình.
