# Qunxiong · Mac 试玩版

Qunxiong 是开发代号，正式名还没定。

一款三国题材的肉鸽策略游戏。在沙盘格子上摆兵营、武将和军师，战斗自动进行，加成与倍率层层叠加。刘备从白身起家：

- 第一幕沿他一生的 12 场战役打，史实里的败仗打赢了就改写历史。
- 第二幕逐州一统天下，第三幕远征四海。
- 第四幕「万国」一路打到欧罗巴、非洲和新大陆，之后是无尽的「万世」。

这是开发中的试玩版，数值和界面还会改。

## 下载

到 [Releases](https://github.com/gangchen/qunxiong-releases/releases/latest) 下载最新的 `Qunxiong-<版本>-arm64.dmg`。

## 系统要求

- Apple 芯片的 Mac（M1 及以后）。Intel 芯片的 Mac 暂不支持。
- macOS 13 或更新。
- 约 350 MB 磁盘空间。

## 安装

这个版本还没有经过 Apple 公证，第一次打开会被系统拦下，需要手动放行一次：

1. 打开下载的 dmg，把 Qunxiong 拖进「应用程序」文件夹。
2. 双击 Qunxiong，系统提示无法验证时，点「完成」。
3. 打开「系统设置 → 隐私与安全性」，拉到「安全性」一栏，点 Qunxiong 旁边的「仍要打开」。输入开机密码或用触控 ID 确认，再在弹窗里点「打开」。macOS 15 起，「右键 → 打开」已经不能绕过这一步。
4. 如果提示「已损坏，无法打开」，打开「终端」运行下面这行，再双击 Qunxiong：

```bash
xattr -dr com.apple.quarantine /Applications/Qunxiong.app
```

## 说明

- 游戏完全离线，不联网，也不收集任何数据。
- 存档在 `~/Library/Application Support/Qunxiong`，只保存在你自己的电脑上。
- 更新时下载新版 dmg，替换「应用程序」里的旧版即可。存档会保留，新版能读入旧版的存档。
- 下载的文件可以用每个版本发布说明里的 SHA-256 核对：`shasum -a 256 Qunxiong-<版本>-arm64.dmg`。

## 反馈

问题和建议请提到本仓库的 [Issues](https://github.com/gangchen/qunxiong-releases/issues)（需要 GitHub 账号）。

## 许可

本仓库只用来分发试玩安装包，不含源代码。安装包请勿修改或转售。

游戏内的字体 Noto Sans SC、Noto Serif SC、Ma Shan Zheng 和 JetBrains Mono 按 SIL Open Font License 1.1 授权，随包附有许可全文。
