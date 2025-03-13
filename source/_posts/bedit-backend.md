---
title: BEdit后端项目经历总结
date: 2025-03-13 22:07:53
categories:
    - Flask
    - AI
    - DevOps
    - Repos
tags:
    - Flask
    - AI
    - OCR
    - DevOps
---

# BEdit后端项目经历总结

## 技术栈

1. **核心框架与库**
   - Flask - 构建Web API服务
   - erniebot - 集成百度文心一言AI模型
   - PaddleOCR - 实现图像文字识别功能
   - MongoDB - 数据存储

2. **部署与运维**
   - PDM - Python项目依赖管理
   - Waitress - 生产环境WSGI服务器
   - GitHub Actions - CI/CD自动化部署

3. **工具库**
   - Loguru - 日志管理系统
   - Flask-CORS - 处理跨域资源共享
   - pytoml - 项目配置管理

## 技术难点

1. **AI大模型集成**
   - 难点：接入百度文心一言API，实现智能对话功能
   - 解决方法：采用erniebot库封装API调用，实现流式和非流式响应处理，并使用初始化消息列表确保模型身份一致性

2. **OCR图像识别**
   - 难点：需从图片中提取文字内容，支持多语种识别
   - 解决方法：集成PaddleOCR库，封装识别流程，实现高效的图文转换API

3. **异步流式响应**
   - 难点：实现AI模型的实时流式输出，提升用户交互体验
   - 解决方法：使用Flask的stream_with_context和生成器函数，结合erniebot的流式接口实现数据流输出

4. **数据持久化**
   - 难点：聊天历史记录需要高效存储与检索
   - 解决方法：设计封装MongoDB操作的DBHandler类，实现通用数据增删改查功能

5. **日志系统集成**
   - 难点：统一多个库的日志记录行为，便于问题排查
   - 解决方法：使用Loguru配置统一日志格式，通过InterceptHandler拦截并重定向标准日志输出

6. **自动化部署**
   - 难点：简化部署流程，确保版本一致性
   - 解决方法：配置GitHub Actions工作流，使用SSH远程命令实现代码拉取、依赖安装和服务重启

这个项目综合运用了Web开发、AI模型集成和DevOps实践，构建了一个具备智能对话和OCR功能的后端服务，为富文本编辑器提供AI增强能力。