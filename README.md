## Cái này là gì??? ❓❓❓
```
Hello đây là Roadmap của bản thân tôi hãy cùng tham khảo nếu bạn cũng muốn học tập với lập trình nhúng. 
Chúc bạn thành công với sự lựa chọn của mình. 
Nếu cần giúp đỡ hãy liên hệ: `0392176769 💌`
Cảm ơn vì sự ghé thăm của bạn 🥰🥰🥰
```

# 🚀 ROADMAP HỌC ARDUINO

# Leanbot
[Tài liệu tham khảo Arduino](https://www.arduino.cc/reference/en/)

## 📌 MỤC LỤC
- [🔹 GIAI ĐOẠN 1 – LÀM QUEN LẬP TRÌNH & PHẦN CỨNG CƠ BẢN](#-giai-đoạn-1--làm-quen-lập-trình--phần-cứng-cơ-bản)
- [🔸 GIAI ĐOẠN 2.1 – THỰC HÀNH MỞ RỘNG VÀ TƯ DUY MODULE](#-giai-đoạn-21--thực-hành-mở-rộng-và-tư-duy-module)
- [🔷 GIAI ĐOẠN 2.2 – LÀM VIỆC VỚI CẢM BIẾN & ỨNG DỤNG THỰC TẾ](#-giai-đoạn-22--làm-việc-với-cảm-biến--ứng-dụng-thực-tế)
- [🔶 GIAI ĐOẠN 3 – ESP32 & KẾT NỐI KHÔNG DÂY](#-giai-đoạn-3--esp32--kết-nối-không-dây)
- [🔴 PHỤ LỤC – CẤU TRÚC BÁO CÁO DỰ ÁN MẪU](#-phụ-lục--cấu-trúc-báo-cáo-dự-án-mẫu)

---

## 🔹 GIAI ĐOẠN 1 – LÀM QUEN LẬP TRÌNH & PHẦN CỨNG CƠ BẢN

### 1. Nên tìm hiểu điều gì?
- Ngôn ngữ lập trình C cơ bản
- Làm quen Arduino Uno / Nano (sơ đồ chân, vai trò các chân)
- Hiểu rõ sơ đồ chân Arduino, các loại chân (Digital / Analog / PWM / GND / Vin / ...), vai trò của chúng
- Thực hành lập trình cơ bản: LED, nút nhấn, biến trở, buzzer,...
- Làm quen Serial Monitor để in giá trị và debug
- Làm quen GitHub, tư duy tổ chức dự án cá nhân

### 2. Gợi ý tìm hiểu
- C: kiểu dữ liệu, mảng, con trỏ, hàm, điều kiện, vòng lặp,...
- Hàm: định nghĩa, truyền tham số, trả giá trị
- Arduino: pinMode(), digitalWrite(), digitalRead(), analogRead(), Serial.begin(), Serial.print()
- Các loại chân Digital / PWM / Analog trên các mạch Arduino Uno/ Arduino Nano
- Sơ đồ chân của Arduino Uno / Nano: học kỹ từ datasheet
- Linh kiện cơ bản: LED, button, biến trở, buzzer, cảm biến ánh sáng (LDR),...
- Làm quen tư duy tách code ra thành hàm con, viết rõ ràng – dễ hiểu

### 3. Câu hỏi gợi ý tìm hiểu
- Arduino Uno và Nano có gì khác nhau?
- Mỗi loại mạch có bao nhiêu chân digital, analog, PWM?
- Sơ đồ chân Arduino có ý nghĩa gì?
- Các tín hiệu Analog – Digital có ưu nhược điểm gì?
- Cần dùng lệnh pinMode() để làm gì? Khi nào nên dùng INPUT_PULLUP? → Hiểu cơ chế của pin đầu vào (floating, nhiễu) và cách ổn định.
- delay() có nhược điểm gì? Khi nào không nên dùng delay()? 
- Làm sao để tạo một hàm delay không chặn (non-blocking delay)? 
- Làm sao để debounce (chống rung) nút nhấn? → Debounce là gì?
- Debounce là gì? Có các cách debounce nào (delay, millis, thư viện)?
- Tại sao nên tách chương trình thành nhiều hàm nhỏ?
- Serial Monitor là gì? Dùng khi nào? Làm sao để gửi dữ liệu từ Arduino về máy tính? → Tìm hiểu Serial.begin(), tốc độ baudrate, Serial.print()...
- Cách đo điện áp từ biến trở?
- Nối LED sao cho đúng? Vì sao cần điện trở?
- Làm sao để điều chỉnh độ sáng LED?

### 4. Một số bài tập / ứng dụng nên làm:
- Nhấn nút bật/tắt LED
- Debounce nút nhấn
- Điều chỉnh độ sáng LED bằng biến trở
- Phát âm thanh đơn giản với buzzer
- LED nhấp nháy không dùng delay
- Đọc giá trị LDR và hiển thị lên Serial Monitor
- Đếm số lần nhấn nút và in ra Serial
- Làm đồng hồ không blocking sử dụng millis()
- Còi báo sáng – LDR + Buzzer
- Mô phỏng mạch điện bằng Proteus
- Tạo 1 repo GitHub lưu lại toàn bộ code và mô phỏng của bạn (quan trọng)

🔝 [Trở về đầu trang](#-mục-lục)

---

## 🔸 GIAI ĐOẠN 2.1 – THỰC HÀNH MỞ RỘNG VÀ TƯ DUY MODULE

### 1. Nên tìm hiểu điều gì?
- Các IC cơ bản và phân loại chúng
- Làm việc với nhiều module phổ biến
- Học về I2C, SPI, UART
- Cấu trúc chương trình nhiều file, chia thư viện

### 2. Gợi ý tìm hiểu
- IC Logic: AND, OR, NOT,...
- IC Shift Register: 74HC595
- IC Timer: NE555
- IC Đếm: CD4017
- IC Comparator: LM393
- IC Driver: ULN2003, L298N
- IC nguồn: AMS1117, TP4056
- IC điều khiển step motor: A4988, DRV8825
- IC giao tiếp: CH340, CP2102

### 3. Câu hỏi gợi ý tìm hiểu
- Sự khác nhau giữa 74HC595 và 74HC165?
- Cách hoạt động của IC NE555 ở chế độ monostable và astable?
- Driver L298N khác gì ULN2003?
- Khi nào nên dùng IC shift register?
- SPI/I2C/UART là gì? Khác nhau?

### 4. Bài tập / ứng dụng:
- Điều khiển nhiều LED bằng 74HC595
- Làm đồng hồ NE555 + CD4017
- Giao tiếp I2C đọc nhiệt độ từ cảm biến
- Điều khiển step motor qua DRV8825
- Giao tiếp UART giữa hai board Arduino

🔝 [Trở về đầu trang](#-mục-lục)

---

## 🔷 GIAI ĐOẠN 2.2 – LÀM VIỆC VỚI CẢM BIẾN & ỨNG DỤNG THỰC TẾ

### 1. Nên tìm hiểu điều gì?
- Cảm biến siêu âm, DHT11/22, MPU6050, MQ-x, RC522, IR sensor...
- Nguyên lý và cách kết nối
- Cách thu thập, xử lý, lọc tín hiệu

### 2. Gợi ý tìm hiểu
- Giao tiếp từng loại cảm biến
- Lọc nhiễu dữ liệu cảm biến (moving average, median filter...)
- Giới hạn đo, độ chính xác, sai số
- Giao tiếp SPI/I2C/UART tương ứng

### 3. Câu hỏi gợi ý tìm hiểu
- Cảm biến nào phù hợp đo khoảng cách? Nhiệt độ? Khí gas?
- Tín hiệu cảm biến thường bị nhiễu, xử lý sao?
- Sự khác biệt giữa DHT11 và DHT22?
- IR Sensor hoạt động như thế nào?

### 4. Ứng dụng nên làm:
- Đo khoảng cách và hiển thị LCD
- Đọc nhiệt độ – độ ẩm từ DHT11
- Đọc thẻ RFID để mở cửa
- Hệ thống phát hiện vật cản bằng IR + buzzer

🔝 [Trở về đầu trang](#-mục-lục)

---

## 🔶 GIAI ĐOẠN 3 – ESP32 & KẾT NỐI KHÔNG DÂY

### 1. Nên tìm hiểu điều gì?
- Kiến trúc ESP32 và cách dùng
- Kết nối WiFi, Bluetooth
- Giao tiếp MQTT, WebServer đơn giản
- OTA update, SPIFFS, Firebase

### 2. Gợi ý tìm hiểu
- Cách nạp code vào ESP32 bằng Arduino IDE
- Cấu hình kết nối WiFi cơ bản
- Giao tiếp MQTT publish/subscribe
- Tạo web server cơ bản trên ESP32
- OTA cập nhật từ xa
- Tải lên SPIFFS hoặc LittleFS

### 3. Câu hỏi gợi ý tìm hiểu
- ESP32 có mấy core? Tốc độ xử lý? So với Uno?
- Làm sao để kết nối ESP32 vào WiFi?
- WebServer hoạt động thế nào trên ESP32?
- MQTT khác HTTP chỗ nào? Khi nào nên dùng?
- Cách OTA cập nhật phần mềm từ xa

### 4. Bài tập:
- Kết nối ESP32 vào WiFi và gửi dữ liệu lên Firebase
- Xây dựng WebServer với ESP32 điều khiển LED
- Sử dụng MQTT để giao tiếp giữa các thiết bị

🔝 [Trở về đầu trang](#-mục-lục)

---

## 🔴 PHỤ LỤC – CẤU TRÚC BÁO CÁO DỰ ÁN MẪU

```markdown
# Cấu trúc báo cáo:

1. **Mục tiêu dự án:**
    - Giới thiệu mục đích, bài toán giải quyết
2. **Thiết kế hệ thống:**
    - Mô tả sơ đồ khối, linh kiện sử dụng
3. **Cấu trúc phần mềm:**
    - Giới thiệu các thư viện sử dụng
4. **Mã nguồn:**
    - Đưa mã nguồn chi tiết
5. **Giải thích cách thức hoạt động:**
    - Phân tích cách hoạt động của hệ thống
6. **Kết quả & Ứng dụng thực tế:**
    - Kết quả sau khi triển khai
    - Các hướng phát triển thêm
