# 🌐 Local Passport Website

## 📌 Giới thiệu
Dự án này minh họa cách tích hợp **Passport.js (LocalStrategy)** vào một website với **Express.js + MongoDB + EJS template**.  
Ứng dụng cho phép người dùng:
- **Đăng ký (Register)**
- **Đăng nhập (Login)**
- **Xem trang Profile (chỉ khi đăng nhập)**

---

## ⚙️ Cài đặt & Chạy thử

### 1️⃣ Clone repo
```bash
git clone https://github.com/HoaiLoc9/local_passport_website.git
cd local_passport_website
```
## 2️⃣ Cài đặt dependencies
```bash
npm install
```
## 3️⃣ Chạy server
```bash
node app.js
```

### 🔑 Các trang chính
## 1. Register
Truy cập: http://localhost:3000/register

Kết quả: User mới được lưu vào MongoDB với password đã được hash.

![register](https://github.com/HoaiLoc9/Local_passport_website/blob/main/public/results/register4.png?raw=true)

## 2. Login
Truy cập: http://localhost:3000/login

Kết quả:

Nếu đúng → chuyển hướng sang trang Profile.

Nếu sai → hiển thị thông báo lỗi.
![login](https://github.com/HoaiLoc9/Local_passport_website/blob/main/public/results/login4.png?raw=true)
![logincheckdb](https://github.com/HoaiLoc9/Local_passport_website/blob/main/public/results/checkdb4.png?raw=true)

## 3. Profile
Truy cập: http://localhost:3000/profile

Yêu cầu: phải login trước.

Hiển thị thông tin user.
![profile](https://github.com/HoaiLoc9/Local_passport_website/blob/main/public/results/profile4.png?raw=true)

## 📂 Cấu trúc dự án
```bash
local_passport_website/
│── app.js   
│── config/passport.js 
│── models/User.js     
│── routes/auth.js      
│── views/              
│   ├── register.ejs
│   ├── login.ejs
│   ├── profile.ejs
│ 
│── public/results             
│── package.json
│── README.md
```
