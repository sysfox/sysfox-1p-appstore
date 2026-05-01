# OpenPanel

OpenPanel is an open-source web and product analytics platform that combines the power of Mixpanel with the ease of Plausible, and one of the best Google Analytics replacements.

## ✨ Features

- **🔍 Advanced Analytics**: Funnels, cohorts, user profiles, and session history
- **🎬 Session Replay**: Record and replay user sessions with privacy controls built in
- **📊 Real-time Dashboards**: Live data updates and interactive charts
- **🎯 A/B Testing**: Built-in variant testing with detailed breakdowns
- **🔔 Smart Notifications**: Event and funnel-based alerts
- **🌍 Privacy-First**: Cookieless tracking and GDPR compliance
- **🚀 Developer-Friendly**: Comprehensive SDKs and API access
- **📦 Self-Hosted**: Full control over your data and infrastructure
- **🛠️ Custom Dashboards**: Flexible chart creation and data visualization
- **📱 Multi-Platform**: Web, mobile (iOS/Android), and server-side tracking
- **💰 Revenue Tracking**: Monitor purchases, subscriptions, and LTV

## Stack

- **Next.js** - the dashboard
- **Fastify** - event API
- **PostgreSQL** - storing basic information
- **ClickHouse** - storing events
- **Redis** - cache layer, pub/sub and queue

## Usage

After deployment, access the configured dashboard port to start using OpenPanel.

### Important Configuration

1. **Dashboard Port**: Web port for accessing the OpenPanel admin interface
2. **API Port**: Port for receiving tracking data, to be configured in your SDKs
3. **Dashboard Public URL**: Enter your server's actual address (e.g., `http://your-server-ip:port`), used for internal references
4. **Cookie Secret**: Set a random secure string to encrypt session data
5. **Database Password**: PostgreSQL database password, use a strong password

### First Login

On first access to the dashboard, you can register to create an admin account. It is recommended to disable public registration after setup (ALLOW_REGISTRATION=false).

### SDK Integration

Integrate the OpenPanel SDK in your website, pointing the API URL to your API port:

```javascript
import { OpenPanel } from '@openpanel/web';

const op = new OpenPanel({
  clientId: 'your-client-id',
  apiUrl: 'http://your-server-ip:api-port/api',
});
```

## Documentation

For more details, visit: https://openpanel.dev/docs

## Links

- GitHub: https://github.com/Openpanel-dev/openpanel
- Website: https://openpanel.dev
