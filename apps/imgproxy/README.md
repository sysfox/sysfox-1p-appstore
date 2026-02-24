# imgproxy

imgproxy 是一个快速且安全的独立服务器，用于调整大小和转换远程图片。imgproxy 的主要原则是简单、速度和安全性。

## 功能特性

### 🚀 高性能

- **极速处理** - 基于 Go 语言编写，性能卓越
- **内存高效** - 优化的内存使用，适合大规模部署
- **并发处理** - 支持高并发图片处理请求

### 🔒 安全特性

- **URL 签名** - 通过 HMAC 签名防止未授权访问
- **资源限制** - 支持限制图片大小、处理时间等
- **只读操作** - 不存储任何图片，仅处理和转发

### 🖼️ 丰富的处理选项

- **智能裁剪** - 支持多种裁剪模式
- **格式转换** - 支持 WebP、AVIF、PNG、JPEG 等格式
- **尺寸调整** - 灵活的缩放和裁剪选项
- **图片优化** - 自动优化图片质量和大小

### 🔗 多种数据源

- **HTTP/HTTPS** - 从远程 URL 获取图片
- **本地文件系统** - 处理本地图片文件
- **S3 存储** - 支持 Amazon S3 及兼容存储

## 使用说明

部署后，通过以下 URL 格式访问图片：

```
http://your-server:8080/insecure/resize:fill:300:300:1/plain/https://example.com/image.jpg
```

### 安全模式

为了安全起见，建议配置 Key 和 Salt 以启用 URL 签名验证：

1. 生成十六进制密钥：`xxd -g 2 -l 64 -p /dev/random | tr -d '\n'`
2. 在配置中设置 `IMGPROXY_KEY` 和 `IMGPROXY_SALT`

## 文档

更多详细信息，请访问官方文档：https://docs.imgproxy.net

## 项目地址

- GitHub: https://github.com/imgproxy/imgproxy
- 官方网站: https://imgproxy.net
- 官方文档: https://docs.imgproxy.net
