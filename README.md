

# Accommodation Search System

Hệ thống tìm kiếm chỗ ở mạnh mẽ, hiện đại, tích hợp backend & frontend, mang lại trải nghiệm tối ưu cho người dùng!

---

## 📖 Giới Thiệu

Accommodation Search là nền tảng hỗ trợ người dùng tìm kiếm, quản lý và tương tác với các danh sách chỗ ở (nhà trọ, căn hộ, khách sạn, v.v.). Hệ thống này gồm hai phần:

- **Backend:** Xây dựng với Python/Django, cung cấp API RESTful, xử lý dữ liệu, xác thực OAuth2, quản lý người dùng và chỗ ở.
- **Frontend:** Phát triển bằng ReactJS, cung cấp giao diện thân thiện, trực quan, dễ sử dụng, kết nối trực tiếp với backend qua API.

Mục tiêu dự án là tạo ra hệ thống đáng tin cậy, dễ bảo trì, dễ mở rộng, mang lại trải nghiệm tuyệt vời cho người dùng cuối.

---

## 🌟 Tính Năng Chính

### 🔍 Tìm Kiếm Chỗ Ở  
- Tìm kiếm theo vị trí, giá, tiện ích, loại chỗ ở
- Lọc nâng cao, sắp xếp kết quả

### 👤 Quản Lý Người Dùng  
- Đăng ký, đăng nhập, xác thực qua token  
- Quản lý thông tin cá nhân, đổi mật khẩu

### 🏡 Quản Lý Dữ Liệu Chỗ Ở  
- Thêm, sửa, xóa và xem chi tiết chỗ ở  
- Quản lý hình ảnh, tiện ích, trạng thái

### 🌐 API RESTful  
- Kết nối frontend và ứng dụng bên thứ ba  
- Endpoint tiêu chuẩn, bảo mật cao

### ⚡ Hiệu Suất Cao  
- Tối ưu hóa truy vấn, phản hồi nhanh

### 🖥 Giao Diện Người Dùng (Frontend)
- Giao diện React Native thân thiện người dùng   
- Responsive, hỗ trợ cả mobile và desktop  
- Đăng nhập, đăng ký, tìm kiếm, xem/đặt chỗ ở  
- Quản lý danh sách yêu thích, lịch sử giao dịch

---

## 🛠 Công Nghệ Sử Dụng

**Backend**
- Python 3.9+
- Django
- MySQL 8.x+
- OAuth2 (django-oauth-toolkit)

**Frontend**
- React Native
- Redux Toolkit
- Axios (gọi API)
- React Navigation

**Công Cụ Khác**
- pip, Django ORM, Git

---

## ⚙ Hướng Dẫn Cài Đặt

### 1️⃣ Backend

```bash
git clone https://github.com/thien0709/AccommodationSearch.git
cd Accommodation-search-system-BE
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
pip install -r requirements.txt
# Tạo database accommodation_db trong MySQL
python manage.py migrate
python manage.py runserver
```

### 2️⃣ Frontend

```bash
git clone https://github.com/thien0709/AccommodationSearch.git
cd Accommodation_Search_System_FE
npm install
npm start
```

---

## 📂 Cấu Trúc Thư Mục

**Backend**
```
AccommodationSearch/
├── accommodation_app/
│   ├── migrations/
│   ├── templates/
│   ├── admin.py
│   ├── models.py
│   ├── serializers.py
│   ├── urls.py
│   ├── views.py
│   └── ...
├── accommodation_system/
│   ├── settings.py
│   ├── urls.py
│   └── ...
├── manage.py
└── requirements.txt
```

**Frontend**
```
AccommodationSearch-FE/
├── src/
│   ├── components/
│   ├── pages/
│   ├── redux/
│   ├── App.js
│   ├── index.js
│   └── ...
├── public/
├── package.json
└── README.md
```

---

## 📡 Danh Sách API Backend (Một phần)

| Phương Thức | Endpoint                           | Mô Tả                              |
| ----------- | ---------------------------------- | ----------------------------------- |
| GET         | /api/accommodations/               | Lấy danh sách tất cả chỗ ở         |
| POST        | /api/accommodations/               | Thêm một chỗ ở mới                 |
| GET         | /api/accommodations/<id>/          | Xem chi tiết một chỗ ở             |
| PUT         | /api/accommodations/<id>/          | Cập nhật thông tin chỗ ở           |
| DELETE      | /api/accommodations/<id>/          | Xóa một chỗ ở                      |
| POST        | /api/users/register/               | Đăng ký người dùng mới              |
| GET         | /o/authorize/                      | Yêu cầu xác thực OAuth2            |
| POST        | /o/token/                          | Lấy access token OAuth2            |
