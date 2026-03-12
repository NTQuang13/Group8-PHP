# Buggy PHP Lab

Project PHP mini cho sinh viên thực hành tìm lỗi và sửa lỗi.

## Mục tiêu bài tập

Sinh viên cần:


## Tìm tối thiểu 8 lỗi trong source code.
   - `syntax` 
1. `/index`
- dòng 9 thiếu dấu ,
2. `/?page=setting`
- dòng 5 thiếu dấu ,
3. `/?page=report`
- dòng 16 thiếu dấu )
4. `/?page=order`
- dòng 7 thiếu dấu ;
5. `/?page=customer`
- dòng 3 thiếu dấu ;
   - `logic`
6. `/?page=dashboard`
- Doanh thu tính sai (dòng 12)
- Điều kiện stock sai (dòng 19)
7. `/?page=report`\
- chưa khai báo $reportRows = [];
8. `/?page=checkout`
- $discountPercent = 0.1;

## Cách chạy

Yêu cầu:

- PHP 8.1 trở lên

Chạy built-in server:

```bash
php -S localhost:8000
```

Mở trình duyệt:

```text
http://localhost:8000
```

## Các trang cần kiểm tra

- `/` hoặc `/?page=dashboard`
- `/?page=orders`
- `/?page=checkout`
- `/?page=customers`
- `/?page=reports`
- `/?page=settings`


## Kết quả mong đợi

Sau khi sửa xong:

- Tất cả route đều mở được.
- Số liệu trên dashboard hợp lý.
- Danh sách đơn hàng hiển thị đúng.
- Tính toán checkout đúng logic.
- Báo cáo và cài đặt không còn lỗi syntax.
