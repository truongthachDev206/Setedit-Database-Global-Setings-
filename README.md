# Setedit-Database-Global-Setings
Đây là các tập lệnh API có thể sử dụng để tăng hiệu suất CPU và GPU. Kích hoạt chế độ Game Mode và sử dụng các kiết xuất đồ hoạ OpenGL và Vulkan

Trước Khi Bắt Đầu Tối Ưu, Vui Lòng Bạn Hãy Cài Đặt App SetEdit Trên CH Play: https://play.google.com/store/apps/details?id=by4a.setedit22
-------------------------------------------------------------------------------------------------------------------------------------------------
Follow: https://www.facebook.com/truongthach.info

• Note: Nếu Bạn Xoá Ứng Dụng SetEdit Thì Đồng Nghĩa Với Việc Bạn Sẽ Mất Hết Các Dữ Liệu Đã Cài Vào !!!
# Bắt Đầu Thôi
#3 Lệnh Tối Ưu Khởi Động
ro.config.hw_quickpoweron = true
boot.fps = 25 ( Là tốc độ khung hình khi khởi động máy. để 15 được thì càng tốt )

debug.sf.nobootanimation = 1

• Sau đó khởi động lại máy là tận hưởng thành quả nhé !

# Cài Đặt Nâng Cao ( Chủ Yếu Tăng Hiệu Suất )

• Tăng Mật Độ Điểm Ảnh Trên Màn Hình 
display_density_forced = 209

• Tăng Tốc Độ Khởi Động Điện Thoại
boot.fps = 25 ( 25 là fps, tốc độ khung hình khi khởi động máy, ví dụ như logo )

debug.sf.nobootanimation = 1

• Giảm Thời Gian Sử Dụng Pin - Giảm Hiệu Suất Sử Dụng CPU

wifi.supplicant_scan_interval = 120 ( giúp tăng thời gian giữa các lần quét WiFi, tiết kiệm pin và tốc độ CPU )

• Tối Ưu Game - Kiết Xuất Thư Viện Đồ Hoạ OpenGL < Skia > 

Vâng, chắc chắn bạn nào cũng cần nhất là cái này. việc này giúp cho máy trơn tru hơn ban đầu. tối ưu cho điện thoại của chúng ta :D

debug.enabletr = true
debug.qctwa.preservebuf = 1
dev.pm.dyn_samplingrate = 1
video.accelerate.hw = 1
debug.overlayui.enable = 1
debug.egl.hw = 1

debug.egl.prifiler = 1

debug.sf.hw = 1
debug.composition.type = c2d
debug.composition.type = gpu
debug.performance.tuning = 1
logcat.live = disable

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
# Cài Đặt Chế Độ Hiệu Suất Cao Bằng USB && WIFI ADB Debugging ✓

- Cầu Gỡ lỗi ADB Không Dây 

Android Developers

Android Developers

Android Studio


Cầu gỡ lỗi Android (adb) là một công cụ dòng lệnh linh hoạt cho phép bạn giao tiếp với thiết bị.

Lệnh adb hỗ trợ nhiều thao tác trên thiết bị, chẳng hạn như cài đặt và gỡ lỗi ứng dụng. adb cung cấp quyền truy cập vào một shell Unix mà bạn có thể dùng để chạy nhiều lệnh trên thiết bị. Đây là một chương trình ứng dụng-máy chủ bao gồm ba thành phần:

Ứng dụng: sẽ gửi lệnh. Ứng dụng chạy trên máy phát triển của bạn. Bạn có thể gọi ứng dụng qua một dòng lệnh bằng cách phát ra lệnh adb.
Một trình nền (adbd) chạy lệnh trên thiết bị. daemon chạy dưới dạng quy trình trong nền trên từng thiết bị.
Máy chủ (server) quản lý việc giao tiếp giữa ứng dụng và trình nền. Máy chủ chạy dưới dạng quy trình nền trên máy phát triển của bạn.

#Cách Cài Đặt Công Cụ SDK Android Trên Windows 10 Pro 64Bit

adb nằm trong gói Công cụ nền tảng Android SDK. 

Hãy tải gói này xuống bằng Trình quản lý SDK rồi cài đặt gói này tại " android_sdk/platform-tools/." 

Nếu bạn muốn có gói Công cụ nền tảng Android SDK độc lập

- Bấm Vào Liên Kết Bên Dưới Tại Trang Developer Android ™

https://developer.android.com/studio/releases/platform-tools

# Lệnh Khởi Động Gỡ Lỗi Không Dây Trên Android 2.x >> Android 10

- adb thường giao tiếp với thiết bị qua USB

nhưng bạn cũng có thể sử dụng adb qua Wi-Fi. 

Để kết nối một thiết bị chạy Android 10 (API cấp 29) trở xuống

hãy làm theo các bước ban đầu sau đây qua USB:

1 :  Kết nối thiết bị Android và máy tính lưu trữ adb với mạng Wi-Fi chung.

2 : Kết nối thiết bị với máy tính lưu trữ bằng cáp USB.

3 : Đặt thiết bị đích để nghe kết nối TCP/IP trên cổng 5555:

- adb tcpip 5555

4 : Rút cáp USB khỏi thiết bị đích.

5 : Tìm địa chỉ IP của thiết bị Android. Hãy vào cài đặt WIFI để tìm điều này !

6 : Kết nối với thiết bị theo địa chỉ IP của thiết bị.

- adb connect device_ip_address:5555

7 : Xác nhận rằng máy tính lưu trữ của bạn đã kết nối với thiết bị đích.
 
- adb devices

< List of devices attached
device_ip_address:5555 device > 

8 : Nếu bạn thấy số seri thiết bị của bạn xuất hiện trên trình giả lập ADB ( Chúc Mừng Bạn Đã Kết Nối Thành Công ) 

 - Trên là các bước giúp bạn kết nối thiết bị của mình với Trình giả lập ADB trên PC ( Android 2.1 >> Android 10 { API 29 trở xuống } ). Còn các thiết bị Chạy Android 11 trở lên hãy bật gỡ lỗi ADB Qua WIFI trong phần ( Tùy Chọn Dành Cho Nhà Phát Triển )

# Các lệnh ADB Tăng Hiệu Suất Android ( Không Khuyến Cáo Vì Có Thể Ảnh Hưởng Đến Pin Và Ứng Suất Nhiệt Của CPU )

 - Lớp GLES

bookmark_border

Trên các thiết bị chạy Android 10 (API cấp 29) trở lên, bạn có thể sử dụng tính năng phân lớp OpenGL ES (GLES). 

Một ứng dụng có thể gỡ lỗi có thể tải các lớp GLES từ APK của ứng dụng đó, từ thư mục cơ sở của ứng dụng hoặc từ một APK lớp đã chọn.

Cách sử dụng lớp GLES tương tự như cách sử dụng lớp xác thực Vulkan.

- Yêu cầu

Lớp GLES chỉ được hỗ trợ trên các phiên bản GLES 2.0 trở lên.

- Đặt lớp

LayerLoader của GLES tìm kiếm các lớp ở những vị trí sau theo thứ tự ưu tiên:

1. Vị trí hệ thống cho thư mục gốc

Vị trí này yêu cầu quyền truy cập thư mục gốc

- adb root

- adb disable-verity

- adb reboot

- adb root

- adb shell setenforce 0

- adb shell mkdir -p /data/local/debug/gles

- adb push <layer>.so /data/local/debug/gles/

2. Thư mục cơ sở của ứng dụng

Ứng dụng mục tiêu phải là ứng dụng có thể gỡ lỗi hoặc bạn phải có quyền truy cập thư mục gốc:

- adb push libGLTrace.so /data/local/tmp

- adb shell run-as com.android.gl2jni cp /data/local/tmp/libGLTrace.so .

- adb shell run-as com.android.gl2jni ls | grep libGLTrace
libGLTrace.so

3. APK bên ngoài

Xác định ABI của ứng dụng mục tiêu, sau đó cài đặt APK chứa các lớp bạn muốn tải:

- adb install --abi armeabi-v7a layers.apk

4. Trong APK của ứng dụng mục tiêu

Ví dụ sau đây cho thấy cách đặt lớp vào APK của ứng dụng:

- jar tf GLES_layers.apk
lib/arm64-v8a/libGLES_glesLayer1.so
lib/arm64-v8a/libGLES_glesLayer2.so
lib/arm64-v8a/libGLES_glesLayer3.so
lib/armeabi-v7a/libGLES_glesLayer1.so
lib/armeabi-v7a/libGLES_glesLayer2.so
lib/armeabi-v7a/libGLES_glesLayer3.so
resources.arsc
AndroidManifest.xml
META-INF/CERT.SF
META-INF/CERT.RSA
META-INF/MANIFEST.MF

# Bật Lớp Cho Từng Ứng Dụng 

- hoặc trên toàn cục. Các chế độ cài đặt theo từng ứng dụng vẫn tồn tại sau những lần khởi động lại, trong khi các thuộc tính toàn cục sẽ bị xoá khi bạn khởi động lại.

# Enable layers

- adb shell settings put global enable_gpu_debug_layers 1

# Specify target application

- adb shell settings put global gpu_debug_app <Pack_Name>

# Specify layer list (from top to bottom)

# Layers are identified by their filenames, such as "libGLLayer.so"

- adb shell settings put global gpu_debug_layers_gles <layer1:layer2:layerN>

# Specify packages to search for layers

- adb shell settings put global gpu_debug_layer_app <package1:package2:packageN>

# Cách Tắt Lớp Trên Ứng Dụng

# Delete the global setting that enables layers

- adb shell settings delete global enable_gpu_debug_layers

# Delete the global setting that selects target application

- adb shell settings delete global gpu_debug_app

# Delete the global setting that specifies layer list

- adb shell settings delete global gpu_debug_layers_gles

# Delete the global setting that specifies layer packages

- adb shell settings delete global gpu_debug_layer_app
# Cách Bật Lớp Toàn Ứng Dụng 

- adb shell setprop debug.gles.layers <layer1:layer2:layerN>

# Nội dung và mã mẫu trên trang này phải tuân thủ các giấy phép như mô tả trong phần Giấy phép nội dung Github. 

Java và OpenJDK là nhãn hiệu hoặc nhãn hiệu đã đăng ký của Developer Android hoặc đơn vị liên kết của Trương Văn Thạch ✓. 




