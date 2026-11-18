# LinguaFloat Web 原型

## 这是哪一版
可通过 iPhone Safari 打开的网页原型：日语/英语/韩语语音识别，翻译成简体中文，双语字幕显示。

## 重要限制
- 这不是原生 iOS App，也不是系统悬浮窗。
- iOS Safari 可能不支持或限制 Web Speech API；需在目标 iPhone 上实际测试。
- iOS 通常会在网页进入后台时暂停网页麦克风/语音识别，因此无法保证同一台 iPhone 一边运行 YouTube 官方 App、一边持续识别。
- 若要稳定捕获 YouTube App 音频，需要原生 iOS ReplayKit Broadcast Upload Extension，需 Xcode、签名和真机测试；网页无法绕过系统限制。
- 翻译使用 MyMemory 公共 API，受服务可用性、速率限制和隐私政策约束。不要输入敏感内容。

## 如何在 iPhone 上试用
网页必须通过 HTTPS 托管后才能可靠使用麦克风和安装 PWA。把本目录部署到支持静态站点的 HTTPS 托管服务，然后用 Safari 打开网址。
Safari 分享按钮 -> 添加到主屏幕。

## 本地开发
直接打开 index.html 可查看界面，但麦克风、语音识别和 PWA 离线功能通常需要 HTTPS 或 localhost。
