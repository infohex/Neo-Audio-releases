# Neo Audio — 浏览器插件下载 / Browser extension downloads

Neo Audio 是一个浏览器音频处理插件：EQ、低频 / 高频提升、混响、3D 宽度、虚拟环绕，以及基于神经网络声部分离的"虚拟舞台"。
源码仓库是私有的；这里只放打包好的插件，任何人可下载。

Neo Audio is a browser audio-processing extension (EQ, bass / treble enhancement, reverb, 3D width, virtual surround, and a
neural-separation "virtual stage"). The source repository is private; this repository only holds the packaged extensions.

| 浏览器 / Browser | 下载 / Download | 安装说明 / Install |
|---|---|---|
| Chrome（及 Chromium 系 / and Chromium-based） | [chrome/neo-audio-chrome.zip](chrome/neo-audio-chrome.zip) | [chrome/README.md](chrome/README.md) |
| Firefox | [firefox/neo-audio-firefox.zip](firefox/neo-audio-firefox.zip) | [firefox/README.md](firefox/README.md) |

每个目录里始终是最新一版；旧版本看这个仓库的提交历史或 [Releases](../../releases)。
Each directory always holds the latest build; older builds are in the commit history or under Releases.

"虚拟舞台"第一次使用时会从 [Neo-Audio-models](https://github.com/infohex/Neo-Audio-models) 下载一次分离模型（168 MB），之后留在浏览器里。
The "virtual stage" downloads its separation model (168 MB) once from Neo-Audio-models on first use and keeps it in the browser.
