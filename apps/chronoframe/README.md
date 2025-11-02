# ChronoFrame

一个流畅的照片展示和管理应用，支持多种图像格式和大尺寸图像渲染。

## 功能特性

### 🖼️ 强大的照片管理

- **在线管理照片** - 通过 Web 界面轻松管理和浏览照片
- **探索地图** - 在地图上浏览照片位置
- **智能 EXIF 解析** - 自动提取元数据，如拍摄时间、地理位置和相机参数
- **逆地理编码** - 自动识别照片拍摄位置
- **多格式支持** - 支持主流格式，包括 JPEG、PNG、HEIC/HEIF
- **智能缩略图** - 使用 ThumbHash 高效生成缩略图

### 🔧 现代技术栈

- **Nuxt 4** - 基于最新的 Nuxt 框架，支持 SSR/SSG
- **TypeScript** - 完全类型安全
- **TailwindCSS** - 现代 CSS 框架
- **Drizzle ORM** - 类型安全的数据库 ORM

### ☁️ 灵活的存储解决方案

- **多种存储后端** - 支持 S3 兼容存储、本地文件系统

## 使用说明

首次部署后，请访问 Web 界面进行初始化设置。

默认情况下，应用使用内置的 SQLite 数据库。如果需要使用其他数据库（如 PostgreSQL），请在环境变量中配置 `DATABASE_URL`。

## 文档

更多详细信息，请访问官方文档：https://chronoframe.bh8.ga/

## 项目地址

- GitHub: https://github.com/HoshinoSuzumi/chronoframe
- 演示站点: https://lens.bh8.ga
