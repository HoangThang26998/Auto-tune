# Thiết kế Giao diện Plugin (UI/UX)

## 1. Auto-Tune 11 Pro Clone
### Bố cục:
- **Header:** Logo "Manus Auto-Tune", Nút Settings, Display Key/Scale hiện tại (nhận từ Auto-Key).
- **Main Dial (Center):** Vòng tròn lớn hiển thị Pitch hiện tại và nốt mục tiêu.
- **Controls (Left):**
    - **Retune Speed:** Knob từ 0 (Fast/Robot) đến 400 (Slow/Natural).
    - **Flex-Tune:** Knob điều chỉnh độ bám của việc chỉnh tông.
    - **Humanize:** Knob giữ lại các nốt rung nhanh.
- **Controls (Right):**
    - **Natural Vibrato:** Điều chỉnh độ rung tự nhiên.
    - **Formant:** Nút bật/tắt bảo toàn formant.
    - **Transpose:** Dịch chuyển tông tổng thể.
- **Bottom:** Bàn phím Piano hiển thị các nốt đang bị khóa (Remove) hoặc ép (Bypass).

## 2. Auto-Key Clone
### Bố cục:
- **Central Display:** Hiển thị Tông (Key), Thang âm (Scale) và BPM lớn ở giữa.
- **Buttons:**
    - **Send to Auto-Tune:** Nút lớn để gửi dữ liệu sang các plugin Auto-Tune.
    - **Latch:** Giữ kết quả dò được.
- **Visualizer:** Biểu đồ Chromagram hiển thị cường độ của 12 nốt nhạc thời gian thực.
