# Chrome 版 / Chrome build

文件：`neo-audio-chrome.zip`（也适用于 Edge、Brave 等 Chromium 系浏览器）。

## 安装（开发者模式加载）

1. 下载 `neo-audio-chrome.zip`，解压到一个**不会被删掉**的目录（浏览器每次启动都从这个目录读）。
2. 打开 `chrome://extensions`，右上角打开"开发者模式"。
3. 点"加载已解压的扩展程序"，选解压出来的目录（里面有 `manifest.json` 的那一层）。
4. 打开任意有声音的页面，点工具栏上的 Neo Audio 图标；页面底部出现圆钮，点它展开面板。

更新：下载新 zip，解压覆盖同一目录，再到 `chrome://extensions` 点该插件的"重新加载"。

## Install (developer mode)

1. Download `neo-audio-chrome.zip` and unzip it into a folder you will keep (the browser reads it on every start).
2. Open `chrome://extensions` and turn on "Developer mode" (top right).
3. Click "Load unpacked" and pick the unzipped folder (the one containing `manifest.json`).
4. Open any page with sound and click the Neo Audio toolbar icon; a round button appears at the bottom of the page, click it to open the panel.

Update: unzip the new build over the same folder, then click "Reload" on the extension in `chrome://extensions`.

## 说明 / Notes

- 虚拟舞台的 GPU 模式用 WebGPU；没有可用 GPU 时自动用 CPU（多线程 wasm）。
- The virtual stage uses WebGPU in GPU mode and falls back to multi-threaded wasm on the CPU.
