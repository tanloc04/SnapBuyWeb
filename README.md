# 🛒 SnapBuyWeb - E-commerce & Recommendation System

**SnapBuyWeb** là một nền tảng thương mại điện tử được xây dựng bằng **Python (Flask)**, tích hợp hệ thống gợi ý sản phẩm (Recommendation System) sử dụng Machine Learning để cá nhân hóa trải nghiệm người dùng.

![Python](https://img.shields.io/badge/Python-3.10-blue) ![Flask](https://img.shields.io/badge/Flask-2.x-green) ![Machine Learning](https://img.shields.io/badge/ML-Scikit--Surprise-orange)

---

## 📄 Tài liệu dự án (Documentation)

Để hiểu rõ hơn về kiến trúc hệ thống, quy trình nghiệp vụ và các thuật toán được sử dụng, bạn có thể xem chi tiết tại tài liệu dưới đây:

👉 **[TẢI XUỐNG TÀI LIỆU CHI TIẾT DỰ ÁN (.PDF)](./docs/SnapBuyWeb.pdf)**

*(Lưu ý: File tài liệu chứa sơ đồ CSDL, Use Case và giải thích thuật toán gợi ý)*

---

## ✨ Tính năng chính

* **Quản lý người dùng:** Đăng ký, Đăng nhập, Quản lý hồ sơ.
* **Mua sắm trực tuyến:** Xem danh sách sản phẩm, Chi tiết sản phẩm, Giỏ hàng.
* **Hệ thống gợi ý (Recommendation System):**
    * Gợi ý sản phẩm tương tự dựa trên hành vi người dùng (Collaborative Filtering).
    * Sử dụng thư viện `scikit-surprise` và `scikit-learn`.
* **Đánh giá & Bình luận:** Người dùng có thể rate sao và để lại bình luận cho sản phẩm.
* **Lịch sử xem:** Tự động lưu và hiển thị các sản phẩm vừa xem.

---

## 🛠 Công nghệ sử dụng

* **Backend:** Python 3.10, Flask Framework.
* **Database:** SQLite (thông qua SQLAlchemy ORM).
* **Frontend:** HTML5, CSS3, Bootstrap 5, Jinja2 Template.
* **Machine Learning:** Scikit-learn, Pandas, NumPy, Scikit-surprise.

---

## 🚀 Hướng dẫn cài đặt và chạy (Installation)

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
