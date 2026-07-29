# OpenPanel

OpenPanel 是一个开源的 Web 与产品分析平台，融合了 Mixpanel 的强大功能和 Plausible 的易用性，也是最佳的 Google Analytics 替代方案之一。

## ✨ 功能特性

- **🔍 高级分析**：漏斗分析、群组分析、用户画像和会话历史
- **🎬 会话回放**：录制并回放用户会话，内置隐私控制
- **📊 实时仪表盘**：实时数据更新和交互式图表
- **🎯 A/B 测试**：内置变体测试，支持详细数据拆分
- **🔔 智能通知**：基于事件和漏斗的告警
- **🌍 隐私优先**：无 Cookie 追踪，符合 GDPR 规范
- **🚀 开发者友好**：完整的 SDK 和 API 访问
- **📦 自托管**：完全掌控您的数据和基础架构
- **🛠️ 自定义仪表盘**：灵活的图表创建和数据可视化
- **📱 多平台支持**：Web、移动端（iOS/Android）及服务端追踪
- **💰 收入追踪**：监控购买、订阅和 LTV 等收入指标

## 技术栈

- **Next.js** - 仪表盘前端
- **Fastify** - 事件 API
- **PostgreSQL** - 存储基础数据
- **ClickHouse** - 存储事件数据
- **Redis** - 缓存、发布/订阅和队列

## 使用说明

部署后，访问配置的仪表盘端口即可开始使用。

### 重要配置说明

1. **仪表盘端口**：用于访问 OpenPanel 管理界面的 Web 端口
2. **API 端口**：用于接收追踪数据的 API 端口，需在 SDK 中配置
3. **仪表盘公共 URL**：请填写您服务器的实际地址（如 `http://your-server-ip:端口`），用于内部引用
4. **Cookie 密钥**：请设置一个随机的安全字符串，用于加密会话数据
5. **数据库密码**：PostgreSQL 数据库密码，请使用强密码

### 首次登录

首次访问仪表盘时，可以通过注册创建管理员账户。建议注册后在设置中禁用公开注册（ALLOW_REGISTRATION=false）。

### SDK 集成

在您的网站中集成 OpenPanel SDK，将 API URL 指向您的 API 端口：

```javascript
import { OpenPanel } from '@openpanel/web';

const op = new OpenPanel({
  clientId: 'your-client-id',
  apiUrl: 'http://your-server-ip:api-port/api',
});
```

## 文档

更多详细信息，请访问：https://openpanel.dev/docs

## 项目地址

- GitHub: https://github.com/Openpanel-dev/openpanel
- 官方网站: https://openpanel.dev
