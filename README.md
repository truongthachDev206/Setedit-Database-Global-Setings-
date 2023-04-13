# Setedit-Database-Global-Setings
Đây là các tập lệnh API có thể sử dụng để tăng hiệu suất CPU và GPU. Kích hoạt chế độ Game Mode và sử dụng các kiết xuất đồ hoạ OpenGL và Vulkan
• Trước Khi Bắt Đầu Tối Ưu, Vui Lòng Bạn Hãy Cài Đặt App SetEdit Trên CH Play: https://play.google.com/store/apps/details?id=by4a.setedit22
-------------------------------------------------------------------------------------------------------------------------------------------------
Follow: https://www.facebook.com/truongthach.info
• Note: Nếu Bạn Xoá Ứng Dụng SetEdit Thì Đồng Nghĩa Với Việc Bạn Sẽ Mất Hết Các Dữ Liệu Đã Cài Vào !!!
# Bắt Đầu Thôi !
3 Lệnh Tối Ưu Khởi Động
ro.config.hw_quickpoweron = true
boot.fps = 25 ( Là tốc độ khung hình khi khởi động máy. để 15 được thì càng tốt )
debug.sf.nobootanimation = 1
Sau đó khởi động lại máy là tận hưởng thành quả nhé !

# Cài Đặt Nâng Cao ( Chủ Yếu Tăng Hiệu Suất )
• Tăng Mật Độ Điểm Ảnh Trên Màn Hình 
display_density_forced = 209
• Tăng Tốc Độ Khởi Động Điện Thoại
boot.fps = 25 ( 25 là fps, tốc độ khung hình khi khởi động máy, ví dụ như logo )
debug.sf.nobootanimation = 1
• Giảm Thời Gian Sử Dụng Pin - Giảm Hiệu Suất Sử Dụng CPU
wifi.supplicant_scan_interval = 120 ( giúp tăng thời gian giữa các lần quét WiFi, tiết kiệm pin và tốc độ CPU )
• Tối Ưu Game - Kiết Xuất Thư Viện Đồ Hoạ OpenGL < Skia > 
Vâng, Hẳn là vậy rồi. chắc chắn bạn nào cũng cần nhất là cái này. việc này giúp cho máy trơn tru hơn ban đầu. tối ưu cho điện thoại của chúng ta :D

debug.enabletr = true
debug.qctwa.preservebuf = 1
dev.pm.dyn_samplingrate = 1
video.accelerate.hw = 1
debug.overlayui.enable = 1
debug.egl.hw = 1
Debug.egl.prifiler = 1
debug.sf.hw = 1
debug.composition.type = c2d
debug.composition.type = gpu
debug.performance.tuning = 1
Logcat.live = disable
• Tăng Độ Nhạy Cảm Ứng 
windowsmgr.max_events_per_sec = 100
• Tăng Chất Lượng Âm Thanh Out
af.resampler.quality = 255
mpq.audio.decode = true
• Tăng Chất Lượng Internet
net.ipv4.ip_no_pmtu_disc = 0
net.ipv4.route.flush = 1
net.ipv4.tcp_ecn = 0
net.ipv4.tcp_fack = 1
net.ipv4.tcp_mem = 187000 187000 187000
net.ipv4.tcp_moderate_rcvbuf = 1
net.ipv4.tcp_no_metrics_save = 1
net.ipv4.tcp_rfc1337 = 1
net.ipv4.tcp_rmem = 4096 39000 187000
net.ipv4.tcp_sack = 1
net.ipv4.tcp_timestamps = 1
net.ipv4.tcp_window_scaling = 1
net.ipv4.tcp_wmem = 4096 39000 18700
• Kích Hoạt Zram ( Ram Ảo )
zram_enabled = 1
---------- Hết ----------
# Tùy Chọn Cấu Hình Qua ADB Debugging Khá Phức Tạp Nên Mình Hướng Dẫn Sau Nhé !!!




