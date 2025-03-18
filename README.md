<h1 align="center">NHẬN DIỆN CỬ CHỈ CÁNH TAY BẰNG CẢM BIẾN GIA TỐC </h1>

<div align="center">

<p align="center">
  <img src="image/logo.png" alt="DaiNam University Logo" width="200"/>
  <img src="image/AIoTLab_logo.png" alt="AIoTLab Logo" width="170"/>
</p>

[![Made by AIoTLab](https://img.shields.io/badge/Made%20by%20AIoTLab-blue?style=for-the-badge)](https://www.facebook.com/DNUAIoTLab)
[![Fit DNU](https://img.shields.io/badge/Fit%20DNU-green?style=for-the-badge)](https://fitdnu.net/)
[![DaiNam University](https://img.shields.io/badge/DaiNam%20University-red?style=for-the-badge)](https://dainam.edu.vn)

</div>

<h2 align="center">Nhận diện cử chỉ cánh tay bằng cảm biến gia tốc</h2>

<p align="left">
  Dự án này tập trung vào việc nhận diện cử chỉ của cánh tay thông qua cảm biến gia tốc MPU6050. Bằng cách sử dụng Machine Learning và AI, hệ thống có thể nhận dạng các cử chỉ khác nhau để ứng dụng vào điều khiển thiết bị thông minh, giao diện người-máy.
</p>
</p>

---

## 🌟 Giới thiệu

- **📌 Thu thập dữ liệu:** Sử dụng cảm biến MPU6050 để thu thập dữ liệu gia tốc và con quay hồi chuyển theo thời gian thực.
- **🤖 Xử lý bằng AI:** Ứng dụng Machine Learning để nhận diện các cử chỉ cánh tay như vẫy, nâng, hạ, xoay...
- **🎮 Ứng dụng thực tế:** Điều khiển thiết bị thông minh, chơi game bằng cử chỉ hoặc hỗ trợ phục hồi chức năng.
- **📊 Lưu trữ và quản lý dữ liệu:** Sử dụng tệp CSV để lưu trữ dữ liệu cảm biến, thuận tiện cho xử lý và huấn luyện mô hình.

---
## 🏗️ HỆ THỐNG
<p align="center">
  <img src="image/He thong.png" alt="System Architecture" width="800"/>
</p>

---
## 📂 Cấu trúc dự án
│── 📁 dulieududoan/         # Dữ liệu để dự đoán cử chỉ  
│── 📁 guidulieu/            # Hướng dẫn xử lý dữ liệu  
│── 📁 image/                # Chứa hình ảnh kết quả  
│── 📁 static/               # File tĩnh cho giao diện web  
│── 📁 templates/            # Giao diện HTML của ứng dụng  
│── 📁 thuchienhanhdong/     # Mã nguồn thực hiện hành động dựa vào nhận diện  
│── 📁 thudulieu/            # Dữ liệu cảm biến thô (CSV)  
│── 📄 .gitignore            # Loại trừ các file không cần thiết khi commit  
│── 📄 README.md             # Mô tả dự án  
│── 📄 confusion_matrix3.png # Hình ảnh ma trận nhầm lẫn của mô hình  
│── 📄 duoanCSV.py           # Code dự đoán từ file CSV  
│── 📄 dulieu1.csv           # Dữ liệu cảm biến thu thập  
│── 📄 label_encoder3.pkl    # File mã hóa nhãn cử chỉ  
│── 📄 lstm_gesture_model3.h5# Mô hình AI đã huấn luyện (LSTM)  
│── 📄 lstm_train.py         # Code huấn luyện mô hình  
│── 📄 scaler3.pkl           # Bộ scaler chuẩn hóa dữ liệu đầu vào  
│── 📄 server4.py            # Server xử lý dự đoán (Flask hoặc API)  
│── 📄 training_history3.png # Hình ảnh lịch sử huấn luyện mô hình  




## 🛠️ CÔNG NGHỆ SỬ DỤNG

<div align="center">

### 🔌 Phần cứng
[![ESP8266](https://img.shields.io/badge/ESP8266-WiFi%20Module-blue?style=for-the-badge)](https://www.espressif.com/en/products/socs/esp8266)
[![MPU6050](https://img.shields.io/badge/MPU6050-IMU-green?style=for-the-badge)](https://invensense.tdk.com/products/motion-tracking/6-axis/mpu-6050/)
[![LED](https://img.shields.io/badge/LED-Indicator-yellow?style=for-the-badge)]()
[![LED Hồng Ngoại](https://img.shields.io/badge/Infrared_LED-5mm-red?style=for-the-badge)]()

### 🖥️ Phần mềm
[![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-Microservice%20API-black?style=for-the-badge&logo=flask)](https://flask.palletsprojects.com/)
[![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-orange?style=for-the-badge)](https://numpy.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Processing-blue?style=for-the-badge)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green?style=for-the-badge)](https://matplotlib.org/)

</div>

## 🛠️ YÊU CẦU HỆ THỐNG

### 🔌 Phần cứng
- **ESP8266** (hoặc ESP32) để thu thập dữ liệu từ cảm biến.
- **MPU6050** - Cảm biến gia tốc và con quay hồi chuyển.
- **LED chỉ báo** để hiển thị trạng thái nhận diện cử chỉ.
- **LED hồng ngoại** (tùy chọn) để hỗ trợ một số chức năng điều khiển.

### 💻 Phần mềm
- **🐍 Python 3+** (Yêu cầu thư viện: NumPy, Pandas, Flask, TensorFlow, Scikit-learn, Matplotlib).
- **📡 Flask Server** để xử lý dữ liệu và dự đoán cử chỉ.
- **📊 CSV** để lưu trữ dữ liệu đầu vào và đầu ra của mô hình.

## 📦 CÁC THƯ VIỆN PYTHON CẦN THIẾT

Để chạy dự án, bạn cần cài đặt các thư viện sau bằng lệnh:

pip install numpy pandas flask tensorflow scikit-learn matplotlib pyserial



## 📖 Hướng dẫn sử dụng  

### 🖐️ Điều khiển TV bằng cử chỉ tay  
1️⃣ **Chuyển kênh** 🔄  
   - **Sang phải** → Tăng kênh 📡  
   - **Sang trái** → Giảm kênh 🔄  

2️⃣ **Tăng/Giảm âm lượng** 🔊🔉  
   - **Nâng tay lên trên** ⬆️ → Tăng âm lượng 🔊  
   - **Hạ tay xuống dưới** ⬇️ → Giảm âm lượng 🔉  

---

### 💡 Điều khiển đèn bằng cử chỉ tay  
1️⃣ **Bật đèn** 💡  
   - **Nâng tay lên trên** ⬆️ → Đèn bật.  

2️⃣ **Tắt đèn** 🌑  
   - **Hạ tay xuống dưới** ⬇️ → Đèn tắt.  

---

### ⚙️ Lưu ý  
- Đảm bảo **ESP8266** đã kết nối với **WiFi** và nhận tín hiệu từ **MPU6050**.  
- Khi thực hiện cử chỉ, giữ tư thế ổn định để tránh sai lệch.  
- Nếu hệ thống không phản hồi, kiểm tra kết nối với **Flask Server**.  
 

## 📰 Poster
<p align="center">
  <img src="image/poster.png" alt="System Architecture" width="800"/>
</p>

## 🤝 Đóng góp
Dự án được phát triển bởi 4 thành viên:

| Họ và Tên              | Vai trò                                                                 |
|------------------------|------------------------------------------------------------------------|
| Phan Đình Quang Vinh  | Phát triển toàn bộ mã nguồn, kiểm thử, triển khai dự án, PowerPoint, và thực hiện video giới thiệu. |
| Bạch Công Quân        | Biên soạn tài liệu Overleaf, Poster,  thuyết trình, đề xuất cải tiến, và hỗ trợ bài tập lớn. |
| Nguyễn Viết Trọng     | Hỗ trợ bài tập lớn, đề xuất cải tiến. |
| Nguyễn Thị Linh Chi   | Hỗ trợ bài tập lớn, PowerPoint, thực hiện video giới thiệu. |


© 2025 NHÓM 6, CNTT16-02, TRƯỜNG ĐẠI HỌC ĐẠI NAM
