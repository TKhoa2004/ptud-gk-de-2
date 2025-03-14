# ptud-gk-de-2
# README - Quản lý công việc

## 1. Thông tin cá nhân
- **Tên:** Trần Anh Khoa  
- **MSSV:** 22000915  

## 2. Thông tin project
### Mô tả
Dự án "Quản lý công việc" là một ứng dụng web giúp người dùng tạo, quản lý và theo dõi tiến độ công việc. Các chức năng chính bao gồm:
- Đăng ký/đăng nhập user
- Thêm/sửa/xóa task
- Theo dõi trạng thái (status) công việc
- Lưu thời gian tạo (created) và thời gian hoàn thành (finished)
- Quản lý user (Admin)
- Upload avatar hoặc chọn avatar ngẫu nhiên từ https://avatar-placeholder.iran.liara.run/

## 3. Hướng dẫn cài đặt

### 3.1. Cài đặt môi trường
Yêu cầu: Python 3.10+

1. **Clone repo:**
   ```sh
   git clone <repo-link>
   cd <repo-folder>
   ```
2. **Tạo venv và cài đặt dependencies:**
   ```sh
   python -m venv venv
   source venv/bin/activate  # Trên macOS/Linux
   venv\Scripts\activate     # Trên Windows
   pip install -r requirements.txt
   ```

### 3.2. Cài đặt database
1. **Tạo file database:**
   ```sh
   flask db init
   flask db migrate -m "Initial migration"
   flask db upgrade
   ```
2. **Hoặc tạo thủ công:**
   ```python
   from app import app, db
   with app.app_context():
       db.create_all()
   ```

### 3.3. Chạy ứng dụng
```sh
flask run
```

Mở trình duyệt tại: `http://127.0.0.1:5000/`

=======
# ptud-gk-de-2

