# Ech0

Ech0 is a next-generation open-source self-hosted platform designed for individual users. It is ultra-lightweight and low-cost, supporting the ActivityPub protocol to let you easily publish and share ideas, writings, and links. With a clean, intuitive interface and powerful command-line tools, content management becomes simple and flexible. Your data is fully owned and controlled by you, always connected to the world, building your own network of thoughts.

## Features

### ☁️ Atomically Lightweight

- **Less than 15MB memory usage** - Extremely low resource consumption
- **Image size under 40MB** - Fast deployment
- **Single SQLite file storage** - Simple and reliable data management

### 🚀 Instant Deployment

- **Zero configuration** - From installation to operation in just one command
- **No additional dependencies** - Ready to use out of the box
- **Cross-platform support** - Windows, Linux, and ARM devices like Raspberry Pi

### ✍️ Distraction-Free Writing

- **Clean online Markdown editor** - Focus on content creation
- **Rich Markdown plugins** - Support for code highlighting, math formulas, and more
- **Real-time preview** - WYSIWYG editing experience

### 📦 Data Sovereignty

- **All content stored locally** - Complete control over your data
- **RSS feed support** - Easy subscription for readers
- **One-click backup & restore** - Supported in Web, TUI, and CLI modes
- **Automatic background backup** - Worry-free data safety

### 🌍 ActivityPub Federation

- **Connect with Mastodon, Misskey, and more** - Join the Fediverse
- **Decentralized ecosystem** - Break down platform barriers
- **Cross-platform interaction** - Seamless communication with other federated users

### 🎨 Rich Features

- **Built-in Todo management** - Easily manage tasks
- **Music player** - Immersive background music and focus mode
- **Video sharing** - Native support for Bilibili/YouTube videos
- **Quick cards** - Display rich media content like website links and GitHub projects
- **Comment system** - Twikoo integration for instant feedback
- **S3 storage integration** - Native support for S3-compatible object storage
- **OAuth2 integration** - Third-party login and API authorization

### 🔐 Secure & Reliable

- **Multi-account permission management** - Flexible access control
- **Access token management** - One-click generation and revocation
- **Real-time system monitoring** - High-performance WebSocket dashboard
- **Highly available Webhook** - Event-driven automated workflows

## Getting Started

After deployment, access the configured port to start using. The first registered user will be automatically set as administrator.

### Basic Configuration

1. **Service port**: Default is 6277
2. **JWT secret**: Recommended to change to a custom secure secret
3. **Data directory**: All data stored in `/app/data` directory
4. **Backup directory**: Backup files stored in `/app/backup` directory

### Advanced Features

- **ActivityPub Federation**: Bind Ech0 to a domain to automatically join the Fediverse
- **S3 Storage**: Configure S3-compatible storage in settings
- **Comment System**: Enable by entering Twikoo backend URL in settings
- **Ech0 Connect**: Connect multiple Ech0 instances for status synchronization

## Documentation

For more details, please visit the official documentation: https://echo.soopy.cn/

## Links

- GitHub: https://github.com/lin-snow/Ech0
- Official Website: https://echo.soopy.cn/
- Preview: https://memo.vaaat.com/
- Ech0 Hub: https://echohub.soopy.cn/
