# Setedit-Database-Global-Setings-
Đây là các tập lệnh API có thể sử dụng để tăng hiệu suất CPU và GPU. Kích hoạt chế độ Game Mode và sử dụng các kiết xuất đồ hoạ OpenGL và Vulkan

# 3 Lệnh Tối Ưu Khởi Động
ro.config.hw_quickpoweron = true
boot.fps = 25 ( Là tốc độ khung hình khi khởi động máy. để 15 được thì càng tốt )
debug.sf.nobootanimation = 1
Sau đó khởi động lại máy là tận hưởng thành quả nhé !
# Trình cài đặt Setedit nâng cao 
- Chỉnh sửa độ phân giải màn hình
display_density_forced = 209
- Tăng tốc độ khởi động điện thoại
boot.fps = 25 ( 25 là fps, tốc độ khung hình khi khởi động máy, ví dụ như logo )
debug.sf.nobootanimation = 1
- Giảm thời gian sử dụng pin + giảm %CPU
( Có Thể Gây Giảm Hiệu Suất ) 
wifi.supplicant_scan_interval = 120 ( giúp tăng thời gian giữa các lần quét WiFi, tiết kiệm pin và tốc độ CPU )
- Tăng Hiệu Suất Khi Chơi Game ✓
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
- Ép Xung GPU + Kiết Xuất Thư Viện Đồ Hoạ OpenGL 3.2
debug.qc.hardware = true
debug.qctwa.statusbar = 1
debug.qctwa.preservebuf = 1
debug.composition.type = gpu
hw3d.force = 1
hwui.render_dirty_regions = false
hwui.disable_vsync = true
- Cài Đặt Ram + Kích Hoạt Ram Ảo
ro.HOME_APP_ADJ = 1
zram_enabled = 1
- Tăng Chất Lượng Hiển Thị
persist.sys.use_dithering = 1 ( có thể giảm fps và hiệu năng xuống )
---------------------------------------------------------------------

#Cảm Ơn Bạn Đã Xem 
Follow Me : https://www.facebook.com/truongthach.info
# Link Tải Setedit Database 
- https://play.google.com/store/apps/details?id=by4a.setedit22
• Note: Nếu Bạn Xoá Ứng Dụng SetEdit Thì Đồng Nghĩa Với Việc Bạn Sẽ Mất Hết Các Dữ Liệu Đã Cài Đặt Trước Đó !!!
• Trương Văn Thạch ✓ 
