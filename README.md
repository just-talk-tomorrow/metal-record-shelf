# 金属唱片架 · Metal Record Shelf

macOS 桌面唱片架：连接自己的网易云音乐账号，把收藏专辑和喜欢歌曲所属专辑摆在桌面上。

[下载 Apple Silicon 安装包](https://github.com/just-talk-tomorrow/metal-record-shelf/releases/latest)

## 功能

- 手机网易云音乐扫码登录，获取收藏专辑及喜欢歌曲所属专辑并去重。
- 每页最多九张，提供多种架体、彩胶、玻璃晕染和随机摆放效果。
- 点击封面直接唤起本机网易云音乐客户端。
- 数据保存在本机，登录凭据由系统钥匙串管理；发行包不包含制作者账号或收藏。

## 安装

适用于 Apple Silicon（M 系列）和 macOS 14+。解压 ZIP 后把“金属唱片架.app”拖入“应用程序”。应用使用个人临时签名，未经过 Apple 公证。

## 从源码构建

需要 Xcode 命令行工具和 Node.js：

```bash
cd Backend
npm ci
cd ..
bash scripts/build.sh
```

构建脚本会把 Node 运行时和依赖打入应用，最终用户无需另装 Node。第三方组件说明见 `Resources/THIRD_PARTY.txt`。

## 许可

本仓库公开源码，但未另行授予本项目源码或视觉素材的开源许可证；第三方组件继续遵循各自许可证。
