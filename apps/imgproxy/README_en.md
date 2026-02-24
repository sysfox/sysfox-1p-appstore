# imgproxy

imgproxy is a fast and secure standalone server for resizing and converting remote images. The main principles of imgproxy are simplicity, speed, and security.

## Features

### 🚀 High Performance

- **Blazing fast** - Written in Go for excellent performance
- **Memory efficient** - Optimized memory usage for large-scale deployments
- **Concurrent processing** - Handles high-concurrency image processing requests

### 🔒 Security

- **URL signing** - Prevent unauthorized access via HMAC signatures
- **Resource limits** - Limit image sizes, processing times, and more
- **Read-only** - Never stores images, only processes and forwards them

### 🖼️ Rich Processing Options

- **Smart cropping** - Multiple cropping modes
- **Format conversion** - WebP, AVIF, PNG, JPEG, and more
- **Resizing** - Flexible scaling and cropping options
- **Image optimization** - Automatically optimize image quality and size

### 🔗 Multiple Sources

- **HTTP/HTTPS** - Fetch images from remote URLs
- **Local filesystem** - Process local image files
- **S3 storage** - Amazon S3 and compatible storage support

## Getting Started

After deployment, access images using the following URL format:

```
http://your-server:8080/insecure/resize:fill:300:300:1/plain/https://example.com/image.jpg
```

### Secure Mode

For security, configure Key and Salt to enable URL signature verification:

1. Generate a hex key: `xxd -g 2 -l 64 -p /dev/random | tr -d '\n'`
2. Set `IMGPROXY_KEY` and `IMGPROXY_SALT` in the configuration

## Documentation

For more details, please visit the official documentation: https://docs.imgproxy.net

## Links

- GitHub: https://github.com/imgproxy/imgproxy
- Official Website: https://imgproxy.net
- Official Documentation: https://docs.imgproxy.net
