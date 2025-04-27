# 个人技术博客

这是一个基于 [Hexo](https://hexo.io/) 框架和 [Cupertino](https://github.com/MrWillCom/hexo-theme-cupertino) 主题构建的个人技术博客。

[![Hexo](https://img.shields.io/badge/Hexo-blue?style=flat-square&logo=hexo)](https://hexo.io/)
[![GitHub license](https://img.shields.io/github/license/thoulee21/thoulee21.github.io?style=flat-square)](LICENSE)

## 项目概述

本博客用于记录个人的技术文章、项目经历、学习笔记和专业知识分享。内容涵盖以下几个主要方面：

- **项目经历总结**：详细记录过往项目技术栈、实现细节和解决方案
- **技术文档与教程**：包含 Markdown、Pandoc、Cobbler 等工具的使用教程
- **技术知识归纳**：如语义化版本控制、测试用例编写等专业知识整理
- **学术资料与笔记**：大学学习资料和相关专业内容

## 主要特性

- **响应式设计**：适配不同屏幕尺寸的设备
- **暗黑模式支持**：基于 Cupertino 主题的明暗模式切换功能
- **分类与标签系统**：清晰的内容组织和导航
- **搜索功能**：内置全站内容搜索
- **代码高亮**：支持多种编程语言的语法高亮
- **数学公式**：支持 LaTeX 数学公式渲染
- **国际化支持**：中英文内容支持

## 技术栈

- **框架**: [Hexo](https://hexo.io/)
- **主题**: [Cupertino](https://github.com/MrWillCom/hexo-theme-cupertino)
- **部署**: GitHub Pages
- **内容格式**: Markdown

## 本地开发环境搭建

### 前置条件

- Node.js (v12.0.0 或更高版本)
- npm 或 yarn

### 安装步骤

1. 克隆仓库

```bash
git clone https://github.com/thoulee21/thoulee21.github.io.git
cd thoulee21.github.io
```

2. 安装依赖

```bash
npm install
# 或
yarn install
```

3. 本地启动服务

```bash
npm run server
# 或
yarn server
```

4. 在浏览器中访问 `http://localhost:4000` 查看博客

### 常用命令

| 命令              | 描述                                     |
| ----------------- | ---------------------------------------- |
| `hexo clean`      | 清除缓存和已生成的静态文件               |
| `hexo generate`   | 生成静态文件                             |
| `hexo server`     | 启动本地服务器，预览博客                 |
| `hexo deploy`     | 部署网站                                 |
| `hexo new post`   | 创建新文章                               |
| `hexo new draft`  | 创建新草稿                               |

## 内容组织结构

- **posts/repos/**: 项目经历相关文章
- **posts/legacy/**: 传统技术文档与笔记
- **posts/interviews/**: 面试相关内容和总结

## 主题配置

主题配置文件为 `_config.cupertino.yml`，可以修改以下主要配置：

- 导航菜单
- 站点信息
- 社交媒体链接
- 页脚信息
- 代码高亮风格

详细配置参考请查看 [Cupertino 主题文档](https://github.com/MrWillCom/hexo-theme-cupertino/tree/main/docs)。

## 项目特色内容

1. **多项目技术栈详解**
   - React/React Native 项目经验总结
   - Next.js 应用开发记录
   - Python 命令行工具开发笔记
   - Go 语言后端服务实践

2. **专业技术文档**
   - Markdown 语法教程
   - Pandoc 文档转换指南
   - 语义化版本控制规范解析

3. **实用工具教程**
   - Cobbler 部署与使用指南

## 贡献指南

如果您发现任何错误或有改进建议，欢迎提交 Issue 或 Pull Request。

## 许可协议

本项目采用 [MIT License](LICENSE) 许可协议。主题采用原作者许可要求。

---

© 2025 thoulee21. 保留所有权利。