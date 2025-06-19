# API-postman
Thực hành Kiểm thử API với Postman
# 🧪 Báo cáo thử nghiệm API với Postman

## 🎯 Mục tiêu

Thực hiện các thao tác cơ bản với API REST bao gồm:
- `GET`: lấy dữ liệu
- `POST`: gửi dữ liệu mới
- `PUT`: cập nhật dữ liệu

Dùng công cụ **Postman** để gửi yêu cầu đến endpoint:  
🔗 `https://jsonplaceholder.typicode.com/posts`

---

## 🧰 Công cụ & Công nghệ sử dụng

| Công cụ         | Mô tả                           |
|----------------|----------------------------------|
| Postman        | Giao diện gửi yêu cầu HTTP      |
| JSONPlaceholder | API giả lập miễn phí để thử nghiệm |
| RESTful API    | Phương pháp giao tiếp qua HTTP  |
| JSON           | Định dạng dữ liệu trao đổi      |

---

1. GET – Lấy danh sách bài viết

**Mô tả:** Gửi yêu cầu `GET` để lấy tất cả các bài viết từ API.

- **URL:** `https://jsonplaceholder.typicode.com/posts`
- **Phương thức:** `GET`

**Kết quả trả về:**
- Mã phản hồi: `200 OK`
- Dữ liệu: danh sách các bài viết dưới dạng JSON

**Ảnh minh họa:**
![GET](./Screenshot%202025-06-19%20171509.png)


**Trích đoạn JSON kết quả:**

```json
[
  {
    "userId": 1,
    "id": 1,
    "title": "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
    "body": "quia et suscipit..."
  },
  {
    "userId": 1,
    "id": 2,
    "title": "qui est esse",
    "body": "est rerum tempore vitae..."
  }
]
2. POST – Gửi một bài viết mới
Mô tả: Gửi yêu cầu POST để tạo mới một bài viết.

URL: https://jsonplaceholder.typicode.com/posts

Phương thức: POST

Body: (dạng JSON)

json
Sao chép
Chỉnh sửa
{
  "title": "Hello",
  "body": "This is a test post.",
  "userId": 1
}
Kết quả trả về:

Mã phản hồi: 201 Created

ID mới được gán: id = 101

Ảnh minh họa:
![GET](./Screenshot%202025-06-19%20171916.png)


3. PUT – Cập nhật bài viết
Mô tả: Gửi yêu cầu PUT để cập nhật nội dung bài viết có id = 101.

URL: https://jsonplaceholder.typicode.com/posts

Phương thức: PUT

Body:

json
Sao chép
Chỉnh sửa
{
  "title": "Updated title",
  "body": "Updated body",
  "userId": 1
}
Kết quả trả về:

Mã phản hồi: 201 Created

Nội dung trả về là nội dung mới được cập nhật

Ảnh minh họa:
![GET](./Screenshot%202025-06-19%20172530.png)


📌 Tổng kết
Phương thức	Mục đích	Trạng thái
GET	Lấy danh sách bài viết	✅ OK
POST	Gửi bài viết mới	✅ OK
PUT	Cập nhật bài viết	✅ OK