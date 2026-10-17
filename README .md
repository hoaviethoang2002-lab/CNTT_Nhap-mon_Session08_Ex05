# 🚀 SMART-FARM — HỆ THỐNG IoT CHO TRANG TRẠI LAN

> **Hướng dẫn sử dụng** dành cho người nông dân.
> **Smart-Farm giúp bạn** theo dõi môi trường - tưới tự động - cảnh báo kịp thời - tiết kiệm chi phí.
## 1. 📖 Mô tả dự án
**Smart-Farm** là hệ thống IoT kết nối cảm biến, gateway, nền tảng xử lý dữ liệu và ứng dụng di động.
Hệ thống hỗ trợ:
- Theo dõi nhiệt độ và độ ẩm không khí.
- Theo dõi độ ẩm đất, ánh sáng, EC và pH nếu được trang bị cảm biến phù hợp.
- Gửi cảnh báo khi thông số vượt ngưỡng đã thiết lập.
- Điều khiển bơm tưới, quạt thông gió và đèn bổ sung.
- Xem lịch sử dữ liệu và xuất báo cáo.
*Lợi ích:* Giám sát từ xa, phát hiện bất thường kịp thời, tiết kiệm công sức và hỗ trợ đưa ra quyết định dựa trên dữ liệu.
## 2. ⚙️ Hướng dẫn cài đặt
![Sơ đồ Smart-Farm](https://rikkeiedu-storage.s3.ap-southeast-2.amazonaws.com/uploads/editor-images/1787648283613_687ec2e7-229c-4942-a347-080fae59560a.webp)
### 2.1. Hệ thống hoạt động như thế nào
1. **Cảm biến:** thu thập dữ liệu (nhiệt độ, độ ẩm,..)
2. **Gateway** gửi dữ liệu lên Internet
3. **Nền tảng** lưu trữ & xử lý dữ liệu
4. **Ứng dụng** hiển thị và cảnh báo
5. **Thiết bị điều khiển** thực hiện tự động (bơm, quạt, đèn,...)
### 2.2. Hướng dẫn sử dụng ứng dụng
1. **Đăng nhập:** Mở Smart-Farm và nhập tài khoản được cấp.
2. **Xem thông số môi trường:** Mở Trang chủ để kiểm tra nhiệt độ, độ ẩm và các thông số có sẵn.
3. **Nhận cảnh báo:** Mở mục Cảnh báo khi ứng dụng thông báo thông số bất thường.
4. **Điều khiển thiết bị:** Vào mục Thiết bị để bật/tắt thủ công hoặc sử dụng chế độ tự động đã được kiểm thử.
5. **Xem báo cáo:** Chọn ngày, tuần hoặc tháng để xem lịch sử và xuất báo cáo nếu cần.

## 3. ✅ Tính năng và checklist vận hành
### Các tính năng chính
- [x] Thu thập dữ liệu từ cảm biến.
- [ ] Xác nhận cảm biến đã được hiệu chuẩn.
- [ ] Kiểm tra cảnh báo trước khi vận hành thật.
- [ ] Kiểm tra chế độ điều khiển thủ công.
- [ ] Kiểm tra lịch sử dữ liệu và chức năng xuất báo cáo.
### Mẹo sử dụng
- Đặt cảm biến ở vị trí thông thoáng, đúng độ cao của cây Lan.
- vệ sinh cảm biến định kỳ để số liệu chính xác.
- Kiểm tra hệ thống tưới và nguồn nước thường xuyên.
## 4. 📊 Bảng thông số hệ thống

| Thông số | Đơn vị | Mục đích |
|---|---|---|
| Nhiệt độ | °C | Theo dõi nhiệt độ môi trường |
| Độ ẩm không khí | Theo cảm biến| Theo dõi độ ẩm không khí |
| Độ ẩm đất | Theo cảm biến | Hỗ trợ quyết định tưới |
| Ánh sáng | lux | Theo dõi ánh sáng |
| EC | mS/cm | Theo dõi độ dẫn điện dung dịch |
| pH | pH | Theo dõi độ axit/kiềm |
## 5. 🧠 Mô hình DIKW: Từ dữ liệu đến hành động
DIKW là mô hình chuyển hóa dữ liệu thành quyết định có ý nghĩa.
| Cấp độ | Ý nghĩa |
|---|---|
| Data – Dữ liệu | Số đo ban đầu |
| Information – Thông tin | Dữ liệu được đặt trong ngữ cảnh | 
| Knowledge – Tri thức | Hiểu mối quan hệ giữa các yếu tố | 
| Wisdom – Quyết định | Chọn hành động phù hợp và an toàn | 
## 6. 📞 Hỗ trợ kỹ thuật
***Nếu gặp sự cố vui lòng liên hệ:***
:phone: 0988123456
Zalo: Smart-Fram Support
## 7. ⚠️ Lưu ý
- Không tự ý tháo lắp thiết bị khi hệ thống đang hoạt động.
- Ngắt nguồn điện trước khi kiểm tra hoặc bảo trì.
- **RAM đầy:** Ứng dụng có thể phản hồi chậm, bị hệ điều hành dừng hoặc không còn đủ bộ nhớ để xử lý.
	 - **Cách khắc phục an toàn:** Truy cập Terminal và chạy lệnh xóa bộ nhớ đệm log cũ hoặc khởi động lại tiến trình giám sát: 
~~~
sudo systemctl restart smart-farm.service
~~~
- Định kỳ kiểm tra dung lượng thẻ nhớ/RAM và xuất báo cáo dữ liệu cũ ra tệp lưu trữ ngoài.
