# MusicFree - All-in-One 音乐服务器

[![Version](https://img.shields.io/badge/version-1.1.9-blue.svg)](https://github.com/ansgoo/music-free-site/releases)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-飞牛OS-orange.svg)](https://www.fnnas.com/)
[![Arch](https://img.shields.io/badge/arch-x86%20|%20arm-lightgrey.svg)](manifest)

**MusicFree** 是一款集媒体库管理、元数据刮削与插件化扩展于一体的音乐服务器，All-in-One 无损音乐解决方案。

## ✨ 核心特性

### 🎵 音乐管理
- 在线搜索与下载：通过插件订阅注册表，便捷获取无损曲目
- 媒体库管理：扫描入库、去重、在线播放；支持 WebDAV 媒体源
- OpenSubsonic 兼容：支持音流、Supersonic、Symfonium 等客户端接入

### 🎨 元数据刮削
- 单曲 / 专辑 / 艺术家信息补全
- 封面与歌词多源匹配
- 多插件编排，按需组合刮削链路

### 🔌 插件化扩展
- 搜索、刮削、同步能力均通过插件实现
- 订阅注册表，按需安装不同插件组合
- 歌单链接导入与定时同步

### 🎧 歌单同步
- 支持链接导入各平台歌单
- 定时同步，保持曲库最新

## 🐳 部署

Docker 一键部署：

```bash
docker pull ansgoo/music-free:latest
```

数据卷：
- `/app/data` - 配置与数据库
- `/app/music` - 音乐文件

端口：`4533`

## 📚 文档

- 官方文档：https://ansgoo.github.io/music-free-site/
- GitHub：https://github.com/ansgoo/music-free-site

## 📝 更新日志

### V1.1.9
稳定版发布

---
