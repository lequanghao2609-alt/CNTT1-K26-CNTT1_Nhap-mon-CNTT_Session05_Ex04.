# Bài 4: Xử lý lỗi đường dẫn khi triển khai dự án

## 1. Bảng so sánh Absolute Path và Relative Path

| Tiêu chí | Absolute Path | Relative Path |
|---|---|---|
| Ví dụ | `C:\Users\An-K26\FarmProject\data\logs.csv` | `../data/logs.csv` |
| Độ dài | Thường dài hơn | Thường ngắn hơn |
| Tính di động | Thấp, phụ thuộc vào đường dẫn trên máy | Cao hơn, dễ chia sẻ dự án |
| Ưu điểm | Xác định vị trí tệp cụ thể | Linh hoạt khi di chuyển dự án |
| Nhược điểm | Có thể lỗi khi chạy trên máy khác | Phụ thuộc vào vị trí thư mục hiện tại |

## 2. Lựa chọn giải pháp tối ưu

Em chọn Relative Path vì đường dẫn ngắn gọn, dễ bảo trì và thuận tiện khi chia sẻ dự án với người khác.

Ký hiệu `..` có nghĩa là lùi lên một thư mục cha. Với đường dẫn `../data/logs.csv`, chương trình lùi lên thư mục cha rồi truy cập thư mục `data` để đọc tệp `logs.csv`.

## 3. Kết luận

Relative Path giúp tăng tính di động của mã nguồn và thuận tiện khi triển khai dự án trên nhiều máy tính. Tuy nhiên, cần bảo đảm cấu trúc thư mục phù hợp để tránh lỗi đường dẫn.
