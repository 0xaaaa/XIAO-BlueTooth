# XIAO 录音笔 · 网页演示

XIAO nRF52840 Sense 录音笔的 Web Bluetooth 网页工具演示版。

## 在线使用

https://0xaaaa.github.io/XIAO-BlueTooth/

## 使用前提

- **Chrome 或 Edge 浏览器**（Web Bluetooth 目前只有这两种浏览器支持；手机需 Android，桌面 Chrome 也可以）
- 附近有已烧录固件并开机的 XIAO 设备
- 设备 PIN：默认 123456

## 功能

- BLE 连接 + PIN 认证 + 自动授时
- 设备状态实时显示（时间 / 电量 / 心率 / 血氧 / 状态）
- 录音列表、单个/全部下载（IMA ADPCM → WAV，CRC 校验 + 缺口自动补传）
- 下载完成自动标记同步
- 设备端删除录音

> 网页需要 HTTPS 才能调用蓝牙，GitHub Pages 已满足。本地测试可运行 `python -m http.server 8000` 后访问 localhost（仅本地调试，无蓝牙时同样受限）。
