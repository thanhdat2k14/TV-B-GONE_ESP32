# TV-B-Gone for ESP32 (Refactored version made for "ESP32")

**TV-B-Gone** là một thiết bị điều khiển từ xa mini được thiết kế để tắt các TV bằng cách phát các tín hiệu hồng ngoại (IR) phổ biến nhất. Phiên bản này được triển khai sử dụng **ESP32** kết hợp với thư viện **irremoteESP8266**, cho phép phát sóng hồng ngoại linh hoạt và dễ dàng lập trình lại.

---

## Giới thiệu

TV-B-Gone là một dự án mã nguồn mở được tạo ra bởi [Ken Shirriff](http://www.righto.com/2010/03/tv-b-gone-simple-universal-tv-off.html), được phát triển tiếp và tối ưu cho nền tảng ESP8266 bởi tác giả thư viện **irremoteESP8266**.

Thiết bị hoạt động bằng cách phát ra các mã tín hiệu tắt TV phổ biến nhất hiện nay thông qua đèn LED hồng ngoại. ESP8266 với thư viện **irremoteESP8266** cung cấp khả năng xử lý mạnh mẽ và hỗ trợ đa dạng giao thức hồng ngoại, giúp TV-B-Gone phiên bản này hoạt động hiệu quả trên nhiều loại TV khác nhau.

---

## Tính năng chính

- Phát các mã tín hiệu tắt TV phổ biến thông qua đèn LED IR.
- Dùng chip ESP8266 nhỏ gọn, dễ dàng lập trình lại qua WiFi hoặc cổng Serial.
- Tích hợp thư viện **irremoteESP8266** hỗ trợ đa dạng giao thức IR.
- Có thể mở rộng và tùy chỉnh mã tín hiệu theo nhu cầu.
- Nguồn mở, dễ dàng học tập và phát triển.

---

## Yêu cầu phần cứng

- ESP32 (ví dụ ESP Wroom 32D,32U tuỳ bạn,...)
- Đèn LED hồng ngoại (IR LED) x3
- Dây nối, nguồn cấp cho ESP32 và một chút kĩ năng

---

## Cách sử dụng

1. Nạp firmware TV-B-Gone có sử dụng thư viện **irremoteESP8266** vào ESP32.
2. Kết nối LED IR đúng chân GPIO đã cấu hình trong mã nguồn.
(IRLED1=GPIO14,IRLED2=GPIO13,IRLED3=GPIO16)"Sử dụng ít nhất 1-2 LED" để phát tín hiệu
(Check Light=GPIO2 hoặc Led Onboard,TRiGGER PIN=Gpio15,SWITCH=Gpio5)
3. Khi khởi động và bấm nút, ESP32 sẽ phát lần lượt các tín hiệu tắt TV phổ biến.
4. Đèn LED IR sẽ phát tín hiệu đến TV để tắt thiết bị.

---

## Thư viện tham khảo

- [irremoteESP8266 GitHub](https://github.com/crankyoldgit/IRremoteESP8266)

---

## Liên hệ

Nếu bạn có thắc mắc hoặc muốn đóng góp cho dự án, vui lòng liên hệ qua GitHub hoặc email tác giả.

---

## Giấy phép

Dự án được phát hành theo giấy phép MIT. Vui lòng tham khảo file LICENSE để biết thêm chi tiết.

