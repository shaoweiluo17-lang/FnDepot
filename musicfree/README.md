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


端口：`4533`

## 📚 文档

- 官方文档：https://ansgoo.github.io/music-free-site/
- GitHub：https://github.com/ansgoo/music-free-site

## 📝 更新日志

### V1.1.9
稳定版发布

### V1.2.0
- 更新特性
  音乐播放详情页：新增歌曲播放详情页面,点击播放器的专辑封面跳转详情页，支持查看当前播放曲目的详细信息与专辑/艺术家上下文，提升播放体验。
  远程搜索支持乐库音乐：远程搜索插件结果页现已支持同时检索本地乐库，根据检索结果帮助用户决策是否下载。
  心愿管理支持批量拒绝：管理后台 心愿管理 新增批量拒绝功能，管理员可一键勾选并拒绝多条待处理心愿，提升处理效率。
  艺术家头像优化：插件排序逻辑优化，仅使用支持 GetArtistInfo 的插件匹配艺术家头像，提高头像匹配准确度与响应速度。
- 其他改进：
  默认主题色更新为新版视觉规范
  专辑卡片无封面占位背景与歌曲卡片风格统一，并随主题色联动
  图片接口浏览器缓存时间优化，二次加载更快\n-页面宽度优化，提升大屏与小屏的显示效果
  依赖升级：Go 模块与前端依赖集中更新，提升稳定性
- 修复:
  修复并发刮削时 SQLite 锁死问题：优化数据库事务与锁竞争，批量与并发刮削不再因 SQLite busy 中断
  修复批量刮削 SQL 变量超限异常：大量文件同时创建刮削任务时不再报 SQL 变量数量错误
  修复专辑卡片占位与主题不一致的显示问题",

### V1.2.1

- 更新特性
增加了日志导出功能
管理员在用户头像的下拉二级面板中可看到一个日志导出的按钮，点击可导出服务端日志，方便问题定位, 后面大家提问题，建议贴日志附件

- 修复
修复Symfoniym 连接OpenSubSonic协议时，音乐数据同步失败的异常
---
