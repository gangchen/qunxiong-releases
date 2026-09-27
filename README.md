# Qunxiong · 试玩版（Mac / Windows）

Qunxiong 是开发代号，正式名还没定。

一款三国题材的肉鸽策略游戏。在沙盘格子上摆兵营、武将和军师，战斗自动进行，加成与倍率层层叠加。刘备从白身起家：

- 第一幕沿他一生的 12 场战役打，史实里的败仗打赢了就改写历史。
- 第二幕逐州一统天下，第三幕远征四海。
- 第四幕「万国」一路打到欧罗巴、非洲和新大陆，之后是无尽的「万世」。

这是开发中的试玩版，数值和界面还会改。

## 下载

最新版是 **v0.9.2**（2026-09-27）：

| 系统 | 下载 |
|---|---|
| Mac（Apple 芯片） | [Qunxiong-0.9.2-arm64.dmg](https://github.com/gangchen/qunxiong-releases/releases/download/v0.9.2/Qunxiong-0.9.2-arm64.dmg) |
| Windows（64 位） | 安装版 [Qunxiong-0.9.2-x64-setup.exe](https://github.com/gangchen/qunxiong-releases/releases/download/v0.9.2/Qunxiong-0.9.2-x64-setup.exe)（推荐）；免安装版 [Qunxiong-0.9.2-x64.zip](https://github.com/gangchen/qunxiong-releases/releases/download/v0.9.2/Qunxiong-0.9.2-x64.zip) |

历次版本都在 [Releases](https://github.com/gangchen/qunxiong-releases/releases)，每一版的发布说明里写了改动和 SHA-256 校验值。

## 系统要求

**Mac**
- Apple 芯片的 Mac（M1 及以后）。Intel 芯片的 Mac 暂不支持。
- macOS 13 或更新。
- 约 400 MB 磁盘空间。

**Windows**
- Windows 10 或 11，64 位。
- 约 450 MB 磁盘空间。

## 安装

### Mac

这个版本还没有经过 Apple 公证，第一次打开会被系统拦下，需要手动放行一次：

1. 打开下载的 dmg，把 Qunxiong 拖进「应用程序」文件夹。
2. 双击 Qunxiong，系统提示无法验证时，点「完成」。
3. 打开「系统设置 → 隐私与安全性」，拉到「安全性」一栏，点 Qunxiong 旁边的「仍要打开」。输入开机密码或用触控 ID 确认，再在弹窗里点「打开」。macOS 15 起，「右键 → 打开」已经不能绕过这一步。
4. 如果提示「已损坏，无法打开」，打开「终端」运行下面这行，再双击 Qunxiong：

```bash
xattr -dr com.apple.quarantine /Applications/Qunxiong.app
```

### Windows

这个版本还没有做代码签名，第一次运行时 Windows 会提示一次：

1. 双击下载的 `Qunxiong-<版本>-x64-setup.exe`。
2. 如果弹出「Windows 已保护你的电脑」，点「更多信息」，再点「仍要运行」。
3. 按安装向导装好。默认装在当前用户下，不需要管理员权限，也可以改安装位置。装好后从桌面或开始菜单里的 Qunxiong 打开。

不想安装的话，下载 zip，解压到任意文件夹，双击里面的 `Qunxiong.exe`。

## 版本记录

- **v0.9.2**（2026-09-27）：本机排行榜（最远征程、一击封神、最强一战、累计输出、势如破竹，各留前 10 名）；新增 Windows 版（64 位）；安装包不再附带 Steam 组件。
- **v0.9.1**（2026-09-27）：加入音效与音乐；启动先到标题页；新增设置页（全屏、音量、切到别的窗口时静音、战斗回放速度、出征前的结算演出）和「关于」页。
- **v0.8.3**（2026-09-27）：行前排与击穿攻城、开局选主城、每战随机的天时 / 阵法 / 副将 / 敌计、第四幕「万国」、备战界面重做、新增 119 张美术。

## 说明

- 游戏完全离线，不联网，也不收集任何数据。
- 有音效和配乐。「设置」里可以分别调总音量、音乐和音效；切到别的窗口时默认静音，也可以关掉。
- 存档只保存在你自己的电脑上：Mac 在 `~/Library/Application Support/Qunxiong`，Windows 在 `%APPDATA%\Qunxiong`。
- 更新时下载新版，替换旧版即可：Mac 把新版拖进「应用程序」覆盖旧版；Windows 直接运行新版安装程序（免安装版换掉整个文件夹）。存档会保留，新版能读入旧版的存档。
- 下载的文件可以用每个版本发布说明里的 SHA-256 核对：Mac 在「终端」里运行 `shasum -a 256 <文件名>`，Windows 在 PowerShell 里运行 `Get-FileHash <文件名>`。

## 反馈

问题和建议请提到本仓库的 [Issues](https://github.com/gangchen/qunxiong-releases/issues)（需要 GitHub 账号）。

## 许可

本仓库只用来分发试玩安装包，不含源代码。安装包请勿修改或转售。

游戏内的字体 Noto Sans SC、Noto Serif SC、Ma Shan Zheng 和 JetBrains Mono 按 SIL Open Font License 1.1 授权，随包附有许可全文。游戏里的音效和音乐由程序合成，不含第三方音频素材。
