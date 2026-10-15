# Bài 7: Gỡ Lỗi Trang Hướng Dẫn Nộp Bài Của Giảng Viên

## Phần 1. Phân tích lỗi

1. `### Lưu ý quan trọng`: thiếu dấu cách sau `###` → không thành tiêu đề, hiện nguyên chữ `###`.
2. `-Bước 1...` đến `-Bước 4...`: thiếu dấu cách sau `-` → không thành danh sách, các dòng bị gộp thành một đoạn.
3. `[GitHub](github.com)`: thiếu `https://` → thành link tương đối, bấm vào bị lỗi 404.
4. `**HNKS25CNTT1_IT101_Session08`: mở `**` mà không đóng → không in đậm, dấu `**` hiện nguyên.
5. `*Nộp muộn ... điểm!**`: mở 1 dấu `*`, đóng 2 dấu `**` → không khớp, thừa dấu `*` ở cuối.

## Phần 2: Sửa lỗi

```markdown
## Hướng Dẫn Nộp Bài Tập - Session 08

### Lưu ý quan trọng

Các bước nộp bài:

- Bước 1: Tạo tài khoản GitHub tại [GitHub](https://github.com)
- Bước 2: Tạo repository mới đặt tên theo định dạng **HNKS25CNTT1_IT101_Session08**
- Bước 3: Upload file .md của bài làm lên repository
- Bước 4: Copy đường dẫn và nộp lên Portal

> Deadline: Chủ nhật 12:00 — *Nộp muộn sẽ bị trừ 50% điểm!*
```

Quên `https://` thì trình render coi `github.com` là đường dẫn tương đối của trang hiện tại, nên link trỏ tới trang không tồn tại (404) thay vì GitHub thật.
