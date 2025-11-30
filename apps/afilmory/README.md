# Afilmory

Afilmory（/əˈfɪlməri/, "uh-FIL-muh-ree"）是一个为个人摄影网站创造的术语，融合了自动对焦（AF）、光圈（光控制）、胶片（复古媒介）和记忆（捕捉的瞬间）。

一个基于 React + TypeScript 构建的现代照片画廊网站，支持从多种存储源（S3、GitHub）自动同步照片，具有高性能 WebGL 渲染、瀑布流布局、EXIF 信息显示、缩略图生成等功能。

## 安装前置条件

**重要提示：** 安装此应用前，您需要确保已安装以下依赖服务：

- **PostgreSQL 数据库服务** - 请先在应用商店中安装 PostgreSQL 数据库
- **Redis 缓存服务** - 请先在应用商店中安装 Redis 缓存服务

安装时，系统将自动检测并绑定已安装的 PostgreSQL 和 Redis 服务。

## 功能特性

### 🖼️ 核心功能

- **高性能 WebGL 图像渲染器** - 自定义 WebGL 组件，支持流畅的缩放和平移操作
- **响应式瀑布流布局** - 基于 Masonic 驱动，自适应不同屏幕尺寸
- **现代 UI 设计** - 使用 Tailwind CSS 和 Radix UI 组件库构建
- **增量同步** - 智能变更检测，仅处理新增或修改的照片
- **国际化** - 多语言支持
- **OpenGraph** - 社交媒体分享的 OpenGraph 元数据

### 📷 图像处理

- **HEIC/HEIF 格式支持** - 自动转换 Apple 设备的 HEIC 格式
- **TIFF 格式支持** - 自动转换 TIFF 格式
- **智能缩略图生成** - 多尺寸缩略图优化加载性能
- **EXIF 信息显示** - 完整的拍摄参数，包括相机型号、焦距、光圈等
- **Blurhash 占位符** - 优雅的图像加载体验
- **Live Photo 支持** - 检测和显示 iPhone Live Photos
- **HDR 图像支持** - 显示 HDR 图像

### 🎛️ 高级功能

- **富士胶片配方** - 读取和显示富士相机的胶片模拟设置
- **全屏查看器** - 支持手势的图像查看器
- **文件系统标签** - 基于文件系统自动生成标签
- **并发处理** - 多进程/多线程并发处理支持
- **多存储支持** - S3、GitHub 等多种存储后端
- **图像分享** - 分享图像到社交媒体或嵌入 iframe 到您的网站
- **交互式地图浏览器** - 使用 MapLibre 通过 EXIF 数据中的 GPS 坐标实现照片的地理可视化

## 使用说明

部署后需要配置存储后端（S3、GitHub 等）并设置相应的环境变量。

首次部署后，请访问 Web 界面进行初始化设置。

## 文档

更多详细信息，请访问官方文档：https://docs.afilmory.art/

## 项目地址

- 官方网站: https://afilmory.art/
- GitHub: https://github.com/Afilmory/afilmory
- 文档: https://docs.afilmory.art/
