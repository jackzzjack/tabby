[![](docs/readme.png)](https://tabby.sh)


<p align="center">
  <a href="https://github.com/Eugeny/tabby/releases/latest"><img alt="GitHub All Releases" src="https://img.shields.io/github/downloads/eugeny/tabby/total.svg?label=DOWNLOADS&logo=github&style=for-the-badge"></a> &nbsp; <a href="https://nightly.link/Eugeny/tabby/workflows/build/master"><img src="https://shields.io/badge/-Nightly%20Builds-orange?logo=hackthebox&logoColor=fff&style=for-the-badge"/></a> &nbsp; <a href="https://matrix.to/#/#tabby-general:matrix.org"><img alt="Matrix" src="https://img.shields.io/matrix/tabby-general:matrix.org?logo=matrix&style=for-the-badge&color=magenta"></a> &nbsp <a href="https://translate.tabby.sh/"><img alt="Translate" src="https://shields.io/badge/Translate-UI-white?logo=googletranslate&style=for-the-badge&color=white&logoColor=fff"></a> &nbsp; <a href="https://twitter.com/eugeeeeny"><img alt="Twitter" src="https://shields.io/badge/Subscribe-News-blue?logo=twitter&style=for-the-badge&color=blue"></a>
</p>

<p align="center">
  <a href="https://ko-fi.com/J3J8KWTF">
    <img src="https://cdn.ko-fi.com/cdn/kofi3.png?v=2" width="150">
  </a>
</p>

----

### 下載

* [Latest release](https://github.com/Eugeny/tabby/releases/latest)
* [Repositories](https://packagecloud.io/eugeny/tabby): [Debian/Ubuntu-based](https://packagecloud.io/eugeny/tabby/install#bash-deb), [RPM-based](https://packagecloud.io/eugeny/tabby/install#bash-rpm)
* [Latest nightly build](https://nightly.link/Eugeny/tabby/workflows/build/master)

<br/>
<p align="center">
本 README 還適用於以下語言: <a  href="./README.md">:gb: English</a> · <a  href="./README.ru-RU.md">:ru: Русский</a> · <a  href="./README.ko-KR.md">:kr: 한국어</a> · <a  href="./README.zh-CN.md">:cn: 简体中文</a> · <a  href="./README.it-IT.md">:it: Italiano</a> · <a href="./README.de-DE.md">:de: Deutsch</a> · <a href="./README.ja-JP.md">:jp: 日本語</a> · <a href="./README.id-ID.md">:id: Bahasa Indonesia</a>
</p>

----

[**Tabby**](https://tabby.sh) (前身是 **Terminus**) 是一個可高度配置的終端模擬器和 SSH 或串口客戶端，支持 Windows，macOS 和 Linux

* 集成 SSH，Telnet 客戶端和連接管理器
* 集成串行終端
* 定制主題和配色方案
* 完全可配置的快捷鍵和多鍵快捷鍵
* 分體式窗格
* 自動保存標籤頁
* 支持 PowerShell（和 PS Core）、WSL、Git-Bash、Cygwin、MSYS2、Cmder 和 CMD
* 在 SSH 會話中通過 Zmodem 進行直接文件傳輸
* 完整的 Unicode 支持，包括雙角字符
* 不會因快速的輸出而卡住
* Windows 上舒適的 shell 體驗，包括 tab 自動補全（通過 Clink）
* 為 SSH secrets 和設置集成了加密容器
* SSH、SFTP 和 Telnet 客戶端可用作 [Web 應用](https://tabby.sh/app)（也可[託管](https://github.com/Eugeny/tabby-web)）

# 目錄 <!-- omit in toc -->

- [Tabby是什麼](#tabby是什麼)
- [終端特性](#終端特性)
- [SSH 客戶端](#ssh-客戶端)
- [串行終端](#串行終端)
- [便攜式應用](#便攜式應用)
- [插件](#插件)
- [主題](#主題)
- [貢獻](#貢獻)

<a name="about"></a>

# Tabby是什麼

* **Tabby 是** Windows 標準終端 (conhost)、PowerShell ISE、PuTTY、macOS Terminal.app 和 iTerm 的替代品

* **Tabby 不是**一個全新的 shell，也不是 MinGW 或 Cygwin 的替代品。它也不是輕量級的 - 如果你對內存的佔用很敏感，請考慮 [Conemu](https://conemu.github.io) 或 [Alacritty](https://github.com/jwilm/alacritty)
<a name="terminal"></a>

# 終端特性

![](docs/readme-terminal.png)

* 一個 V220 終端 + 各種插件
* 多個嵌套的拆分窗格
* 可以將標籤頁設置在窗口的任意一側
* 帶有全局生成熱鍵的可選可停靠窗口（“Quake console”）
* 進度檢測
* 流程完成通知
* 帶括號的粘貼，多行粘貼提示
* 連體字
* 自定義 shell 配置文件
* 可選的 RMB 粘貼和復制選擇（PuTTY 風格）

<a name="ssh"></a>
# SSH 客戶端

![](docs/readme-ssh.png)

* 帶有連接管理器的 SSH2 客戶端
* X11和端口轉發
* 自動跳轉主機管理
* 代理轉發（包括 Pageant 和 Windows 原生 OpenSSH 代理）
* 登錄腳本

<a name="serial"></a>
# 串行終端

* 保存連接
* 逐行讀取的輸入支持
* 可選的十六進制逐字節輸入和十六進制轉儲輸出
* 換行轉換
* 自動重連

<a name="portable"></a>
# 便攜式應用

如果在 Tabby.exe 所在的目錄創建一個名為`data`文件夾，Tabby 將可以在 Windows 上作為便攜式的應用程序運行。

<a name="plugins"></a>
# 插件

插件和主題可以直接在 Tabby 設置中安裝。

* [clickable-links](https://github.com/Eugeny/tabby-clickable-links) - 使終端中的路徑和 URL 可點擊
* [docker](https://github.com/Eugeny/tabby-docker) - 連接 Docker 容器
* [title-control](https://github.com/kbjr/terminus-title-control) - 允許通過提供要刪除的前綴、後綴和/或字符串來修改標籤頁的標題
* [quick-cmds](https://github.com/Domain/terminus-quick-cmds) - 快速向一個或所有標籤頁發送命令
* [save-output](https://github.com/Eugeny/tabby-save-output) - 將終端輸出記錄到文件中
* [sync-config](https://github.com/starxg/terminus-sync-config) - 將配置同步到 Gist 或 Gitee
* [clippy](https://github.com/Eugeny/tabby-clippy) - 一個可以一直煩你的示例插件
* [workspace-manager](https://github.com/composer404/tabby-workspace-manager) - 允許根據給定的配置創建自定義工作區配置文件
* [search-in-browser](https://github.com/composer404/tabby-search-in-browser) - 從 Tabby 標籤頁帶有選中的文本來打開系統默認瀏覽器

<a name="themes"></a>
# 主題

* [hype](https://github.com/Eugeny/tabby-theme-hype) - 受 Hyper 啟發的主題
* [relaxed](https://github.com/Relaxed-Theme/relaxed-terminal-themes#terminus) - 為 Tabby 打造的 Relaxed 主題
* [gruvbox](https://github.com/porkloin/terminus-theme-gruvbox)
* [windows10](https://www.npmjs.com/package/terminus-theme-windows10)
* [altair](https://github.com/yxuko/terminus-altair)

# Sponsors <!-- omit in toc -->

[![](https://assets-production.packagecloud.io/assets/packagecloud-logo-light-scaled-26ce8e96060fddf74afbd4445e63ba35590d4aaa56edc98495bb390ef3cae0ae.png)](https://packagecloud.io)

[**packagecloud**](https://packagecloud.io) 提供了免費的 Debian/RPM 存儲庫託管

<a name="contributing"></a>
# 貢獻

歡迎提交 PR 和插件！

請參閱 [HACKING.md](https://g