# X Media Downloader

一个 Tampermonkey 油猴脚本：在 X（Twitter）页面加一个悬浮面板，一键保存推文视频（.mp4）和原图。

## 功能
- 任意 X 页面（个人主页、信息流、单条推文）显示悬浮控制按钮
- 视频直接合并保存为单个 `.mp4` 文件（自动处理 HLS 分片流）
- 图片按原图分辨率下载
- 批量模式：在信息流中选中多条推文，一次性全部保存
- 无需登录脚本账号、无设置页，只与 X 自己的媒体 CDN 通信

## 安装
1. 安装 [Tampermonkey](https://www.tampermonkey.net/)（Chrome、Edge 或 Firefox 均可）。
2. 打开脚本 raw 地址：
   `https://raw.githubusercontent.com/USER/x-media-downloader/main/x-media-downloader.user.js`
3. 弹出安装提示 → 点「安装」（也可以手动复制粘贴到 Tampermonkey 新建脚本）。
4. 刷新 x.com 即可。

页面右下角会出现一个小 ⬇ 按钮。

## 使用
1. 点悬浮按钮打开面板。
2. 选中目标推文（批量时可多选）。
3. 点「⬇ 媒体」——视频保存为 `<推文ID>.mp4`，图片逐张保存。

## 常见问题
**点了没反应。** 稍等 1 秒再点——视频需要先播放过一次，流的元信息才会加载出来。

**Firefox 用户。** 请确认浏览器代理设置为「不代理」，否则面板可能不显示。

## 隐私
脚本完全运行在你的浏览器本地，不收集、不上传任何个人数据；唯一的网络请求是向 X 自己的媒体 CDN 拉取你要下载的文件。

## 许可证
MIT
