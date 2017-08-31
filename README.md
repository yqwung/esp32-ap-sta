# 简介   
ESP32 WIFI工作在AP+STA(softAP+station)模式。
# 基于esp-idf-v2.1版本
官方idf链接：[https://github.com/espressif/esp-idf/releases/](https://github.com/espressif/esp-idf/releases/)<br />
# 使用说明
1 更改Makefile中esp-idf的路径为你自己的存放路径或者改环境变量
<pre><code>
# your esp-idf path
IDF_PATH = /home/wang/share/esp32/esp-idf-v2.1
</code></pre>
2 更改user_wifi_ap_sta.h文件中WIFI信息
<pre><code>
// STA
#define WIFI_SSID               "yourwifi"
#define WIFI_PASS               "wifipassword"

// AP
#define ESP32_AP_SSID           "espwifi"      // 设置wifi名
#define ESP32_AP_PASS           "esp123456"    // 设置的wifi 密码必须大于等于8个字符
</code></pre>
3 make编译
