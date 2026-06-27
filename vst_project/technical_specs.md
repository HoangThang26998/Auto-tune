# Tài liệu Kỹ thuật: HT Audio 98 VST Suite

## 1. HT Audio 98 - Auto-Key
### Tính năng nâng cao:
- **Continuous Auto-Detection:** Plugin không chỉ dò một lần mà liên tục phân tích tín hiệu đầu vào để cập nhật tông nếu có sự thay đổi trong bài hát.
- **Auto-Send Engine:** Khi phát hiện tông mới, plugin sẽ tự động gửi thông tin Key/Scale đến tất cả các instance của Auto-Tune 11 Pro trong cùng một project DAW thông qua giao thức MIDI CC/Inter-Plugin Communication.
- **Smart Key Lift:** Tích hợp bộ đếm thời gian từ Playhead của DAW. Khi bài hát đạt đến đoạn cao trào cuối cùng (thường là 10% cuối), plugin sẽ tự động gửi lệnh tăng 1-2 bán âm để tạo hiệu ứng "lên tông" (Modulation) một cách mượt mà.

## 2. HT Audio 98 - Auto-Tune 11 Pro
### Tính năng:
- **Harmony Player:** Tạo bè 4 giọng tự động dựa trên Key nhận được từ Auto-Key.
- **Real-time Pitch Correction:** Thuật toán độ trễ cực thấp cho phép hát live.
- **Formant & Throat Modeling:** Cho phép thay đổi đặc tính giọng hát (nam sang nữ, trẻ con sang người lớn).

## 3. Cách thức hoạt động của Smart Key Lift
1. Auto-Key nhận thông tin thời gian từ DAW.
2. Khi đến điểm kích hoạt (Trigger Point), Auto-Key gửi lệnh `Key_Change_Event`.
3. Auto-Tune nhận lệnh và thực hiện `Slew_Rate_Pitch_Shift` để chuyển tông mà không gây ra tiếng click hoặc artifact.
