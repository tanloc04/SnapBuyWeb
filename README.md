# SnapBuyWeb - E-commerce & Recommendation System

**SnapBuyWeb** là một nền tảng thương mại điện tử được xây dựng bằng **Python (Flask)**, tích hợp hệ thống gợi ý sản phẩm (Recommendation System) sử dụng Machine Learning để cá nhân hóa trải nghiệm người dùng.

![Python](https://img.shields.io/badge/Python-3.10-blue) ![Flask](https://img.shields.io/badge/Flask-2.x-green) ![Machine Learning](https://img.shields.io/badge/ML-Scikit--Surprise-orange)

---

## Tài liệu dự án (Documentation)

Để hiểu rõ hơn về kiến trúc hệ thống, quy trình nghiệp vụ và các thuật toán được sử dụng, bạn có thể xem chi tiết tại tài liệu dưới đây:

**[TẢI XUỐNG TÀI LIỆU CHI TIẾT DỰ ÁN (.PDF)](./docs/SnapBuyWeb.pdf)**

*(Lưu ý: File tài liệu chứa sơ đồ CSDL, Use Case và giải thích thuật toán gợi ý)*

---

## Tính năng chính

* **Quản lý người dùng:** Đăng ký, Đăng nhập, Quản lý hồ sơ.
* **Mua sắm trực tuyến:** Xem danh sách sản phẩm, Chi tiết sản phẩm, Giỏ hàng.
* **Hệ thống gợi ý (Recommendation System):**
    * Gợi ý sản phẩm tương tự dựa trên hành vi người dùng (Collaborative Filtering).
    * Sử dụng thư viện `scikit-surprise` và `scikit-learn`.
* **Đánh giá & Bình luận:** Người dùng có thể rate sao và để lại bình luận cho sản phẩm.
* **Lịch sử xem:** Tự động lưu và hiển thị các sản phẩm vừa xem.

---

## Công nghệ sử dụng

* **Backend:** Python 3.10, Flask Framework.
* **Database:** SQLite (thông qua SQLAlchemy ORM).
* **Frontend:** HTML5, CSS3, Bootstrap 5, Jinja2 Template.
* **Machine Learning:** Scikit-learn, Pandas, NumPy, Scikit-surprise.

---

## Application UI (Giao diện ứng dụng)

### 1. Customer Storefront (Giao diện Khách hàng)
Giao diện mua sắm dành cho người dùng cuối, tích hợp hệ thống gợi ý sản phẩm.

<p align="center">
  <img src="https://github.com/tanloc04/SnapBuyWeb/raw/main/assests/snapbuy_homepage.gif" width="100%" alt="Homepage Demo" />
</p>

**Chi tiết các trang chức năng:**
<p align="center">
  <img src="https://github.com/user-attachments/assets/9c67bef4-a4c3-41e2-99e8-4f9fee9fedda" width="48%" alt="Market Page" />
  <img src="https://github.com/user-attachments/assets/7582127c-0438-431e-af3f-473904da336d" width="48%" alt="Category Page" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/56224ac6-637c-410b-9886-b8114b517e48" width="48%" alt="Shopping Cart" />
  <img src="https://github.com/user-attachments/assets/42c8f981-04cb-4d90-8af0-c83e20e37c72" width="48%" alt="User Profile" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/fcd9dfdf-e474-4d97-b1d0-a36a5dd7fe41" width="48%" alt="News Page" />
  <img src="https://github.com/user-attachments/assets/d361d84d-4b0c-44d4-ae15-52d402557d4a" width="48%" alt="About Us" />
</p>

---

### 2. Admin Dashboard (Giao diện Quản trị)
Hệ thống quản lý dành cho quản trị viên để kiểm soát sản phẩm, danh mục và đơn hàng.

<p align="center">
  <img src="https://github.com/tanloc04/SnapBuyWeb/raw/main/assests/snapbuy_admin_dashboard.gif" width="100%" alt="Admin Demo" />
</p>

**Chi tiết các trang quản lý:**
<p align="center">
  <img src="https://github.com/user-attachments/assets/d367c750-7573-4847-b407-baad3737631f" width="48%" alt="Admin Dashboard" />
  <img src="https://github.com/user-attachments/assets/2291316d-42ee-4dd9-a72a-20c8ddc8f5a9" width="48%" alt="Admin Orders" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/34df5409-704d-48cf-b81f-d82bb6cc0d3d" width="48%" alt="Product Items Management" />
  <img src="https://github.com/user-attachments/assets/5658a569-b8db-476c-8d64-8ee3399af4d2" width="48%" alt="Brands Management" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/547c38ee-1211-4547-a03c-f5d6e18aea99" width="48%" alt="Categories Management" />
  <img src="https://github.com/user-attachments/assets/20262c0a-ada0-417a-bc8b-0fd288bc0798" width="48%" alt="Users Management" />
</p>

---

## Hướng dẫn cài đặt và chạy (Installation)

Làm theo các bước sau để chạy dự án trên máy của bạn:

### 1. Clone dự án
```bash
git clone [https://github.com/tanloc04/SnapBuyWeb.git](https://github.com/tanloc04/SnapBuyWeb.git)
cd SnapBuyWeb
```
### 2. Tạo môi trường ảo (Virtual Environment)
**Trên Windows:**
```bash
python -m venv venv
.\venv\Scripts\activate
```
**Trên macOS/Linux:**
```
python3 -m venv venv
source venv/bin/activate
```

### 3. Cài đặt thư viện
```bash
pip install -r requirements.txt
```
### 4. Chạy ứng dụng
```bash
python run.py
```
