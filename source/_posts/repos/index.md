---
title: 项目经历总结
categories:
  - Repos
  - 简历
date: 2025-03-14 16:07:59
tags:
  - 技术
  - 项目经历
  - 简历
---

# 项目经历总结

## Film Speak 影音学习应用（2024.11-2025.02）
**技术栈**：React Native, TypeScript, ffmpeg-kit, Microsoft Speech SDK, Redux, Expo Router

**项目描述**：跨平台视频学习工具，支持视频处理、语音识别与字幕生成功能。

**主要贡献**：
- 利用ffmpeg-kit在设备本地实现视频转码、剪辑与格式转换，并开发分块处理机制避免内存溢出
- 集成微软认知服务语音SDK，开发字幕同步算法确保视频与文本精准匹配
- 使用react-native-mmkv替代AsyncStorage，显著提升存储性能
- 设计离线工作模式与在线同步机制，确保核心功能在无网络环境下可用

## BEdit 富文本编辑器（2024.09-2024.12）
**技术栈前端**：Next.js 14, React 18, Material UI, EditableJS, Emotion  
**技术栈后端**：Flask, erniebot, PaddleOCR, MongoDB

**项目描述**：一款支持AI辅助写作与OCR识别功能的现代富文本编辑器。

**主要贡献**：
- 前端：基于EditableJS框架设计插件化架构，实现富文本编辑、格式化和协作功能
- 前端：集成docxyz库实现多种文件格式间的无损转换与导入导出
- 后端：封装百度文心一言API接口，实现智能对话功能与流式响应输出
- 后端：集成PaddleOCR实现高效的多语种图文识别转换
- 配置GitHub Actions工作流，实现前后端代码的自动化部署

## NeteaseCmd 命令行音乐客户端（2024.08-2024.10）
**技术栈**：Python, MongoDB, RESTful API, Rich, SnowNLP, PyYAML

**项目描述**：功能丰富的网易云音乐命令行客户端，支持音乐搜索下载、歌单管理等功能。

**主要贡献**：
- 实现WebAPICheck系统监控接口健康状态，自动禁用不可用API
- 设计基于角色(admin/user/visitor)和分组(basic/music/user/accounting)的权限系统
- 扩展Python cmd模块，增强命令行功能与自动补全系统
- 使用MongoDB实现用户数据的跨设备同步与云端自动备份
- 集成SnowNLP实现音乐评论情感分析功能

## Go语言AI聊天机器人（2024.06-2024.08）
**技术栈**：Go 1.24, Gin, GORM, MySQL, Azure OpenAI API, Docker

**项目描述**：基于Go语言的高性能AI聊天服务，集成Azure OpenAI大语言模型能力。

**主要贡献**：
- 采用Server-Sent Events (SSE)技术实现AI回复的实时流式传输
- 基于UUID设计会话管理系统，实现多轮对话上下文的连贯性维护
- 构建AIService抽象层封装Azure OpenAI复杂接口，简化业务逻辑集成
- 设计多阶段构建Dockerfile与Docker Compose配置，优化开发和生产环境一致性

## Joint Player 音乐播放器应用（2024.04-2024.06）
**技术栈**：React Native, Redux Toolkit, SWR, MMKV, React Navigation, React Native Track Player

**项目描述**：跨平台移动音乐播放器应用，支持多源音乐播放、歌词同步和后台播放功能。

**主要贡献**：
- 开发基于MMKV的高性能缓存系统，实现LRU缓存淘汰策略和优先级缓存机制
- 封装TrackPlayer服务，实现音频后台播放、自动队列恢复和歌词同步显示功能
- 通过useThrottle和useDebounce自定义Hooks优化高频函数调用，提升应用流畅度
- 实现fetchPlus和retryFetcher工具，集成第三方音乐API并处理网络波动情况

## 君颖投资企业官网（2024.05-2024.07）
**技术栈**：React 18, React Router 6, SCSS/SASS, GitHub Actions

**项目描述**：响应式企业官网，支持多设备尺寸适配与动态交互效果。

**主要贡献**：
- 实现自定义`flexible.js`脚本，基于设计稿（1920px）将px统一转换为rem单位
- 开发滚动视差效果和过渡动画，提升用户视觉体验
- 使用GitHub Actions工作流实现代码push后自动构建和SFTP部署
- 优化自定义字体加载策略，提升首屏渲染性能