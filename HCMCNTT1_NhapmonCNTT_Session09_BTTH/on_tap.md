# Ôn tập

## Phần 3. Hỏi AI đúng cách

### Prompt (Công thức 3 Phần)

````markdown
## Tôi là ai / Bối cảnh
Tôi là sinh viên mới gia nhập CLB Lập trình, tham gia dự án SmartCampus.
Tôi chưa hiểu rõ thuật ngữ **API** khi đọc tài liệu dự án.

## Chủ đề / Nội dung cần xử lý
Giải thích thuật ngữ **API** theo cách đơn giản nhất cho người mới.

## Yêu cầu
- Giải thích bằng một ví dụ đời thường
- Nêu API được dùng như thế nào trong ứng dụng tra cứu lịch học
- Trình bày bằng Markdown: có tiêu đề, chữ đậm cho ý chính và bullet list
- Viết bằng tiếng Việt, câu ngắn

## Không cần
- Không cần code, không cần nói về REST, GraphQL hay các loại API khác
````

### Tóm tắt câu trả lời của AI (đọc 3 bước, 3 câu)

API là người trung gian giữa ứng dụng và máy chủ, giống người phục vụ nhận món từ khách rồi chuyển vào bếp. Trong SmartCampus, ứng dụng gửi mã sinh viên qua API và nhận lại lịch học để hiển thị. Nhờ API, nhiều ứng dụng dùng chung dữ liệu mà không cần truy cập thẳng vào nơi lưu trữ.

Câu trả lời đầy đủ của AI được lưu trong file `api_giai_thich.md`.

---

## Phần 4. Bẫy cú pháp

### Hai lỗi cú pháp

1. **Bảng thiếu dòng phân cách** `|---|---|` ngay dưới dòng tiêu đề, nên parser không nhận ra đây là bảng.
2. **Task list thiếu dấu cách sau dấu `-`**: viết `-[x]` và `-[ ]` thay vì `- [x]` và `- [ ]`, nên parser không nhận ra đây là task list.

### Đoạn đã sửa

```markdown
| Tính năng | Trạng thái |
|---|---|
| Tra cứu lịch học | Xong |
| Push notification | Đang làm |

- [x] Tra cứu lịch học
- [ ] Push notification
```
