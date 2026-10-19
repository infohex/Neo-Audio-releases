# Firefox 版 / Firefox build

文件：`neo-audio-firefox.zip`。

## 安装（临时载入）

正式版 Firefox 只接受经 Mozilla 签名的附加组件，所以这个 zip 目前只能**临时载入**，重启浏览器后要再载一次：

1. 下载并解压 `neo-audio-firefox.zip`。
2. 地址栏打开 `about:debugging#/runtime/this-firefox`。
3. 点"临时载入附加组件…"，选解压目录里的 `manifest.json`。
4. 打开任意有声音的页面，点工具栏上的 Neo Audio 图标；页面底部出现圆钮，点它展开面板。

要长期安装，需要把 zip 送到 addons.mozilla.org 做自分发签名（免费），拿到 `.xpi` 后直接拖进 Firefox 即可；签名版放出来后会在这里更新。

## Install (temporary add-on)

Release builds of Firefox only accept add-ons signed by Mozilla, so for now this zip can only be loaded **temporarily** and must be loaded again after each browser restart:

1. Download and unzip `neo-audio-firefox.zip`.
2. Open `about:debugging#/runtime/this-firefox`.
3. Click "Load Temporary Add-on…" and pick `manifest.json` inside the unzipped folder.
4. Open any page with sound and click the Neo Audio toolbar icon; a round button appears at the bottom of the page, click it to open the panel.

A permanently installable `.xpi` needs self-distribution signing at addons.mozilla.org (free); it will be posted here once available.

## 说明 / Notes

- Firefox 下虚拟舞台只有 GPU 模式（WebGPU）；后台页没有多线程 wasm，CPU 模式不可用。
- "整机 CPU / 整机内存"两格在 Firefox 下显示"不支持"：Firefox 没有读取系统占用的扩展接口。
- On Firefox the virtual stage is GPU-only (WebGPU); the machine CPU / memory readouts show "N/A" because Firefox has no system-info extension API.
