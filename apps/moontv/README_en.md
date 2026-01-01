# MoonTV

> 🎬 **MoonTV** is an out-of-the-box, cross-platform video aggregation player. Built with **Next.js 14** + **Tailwind CSS** + **TypeScript**, it supports multi-source search, online playback, favorites sync, playback history, and local/cloud storage, allowing you to enjoy massive free video content anytime, anywhere.

## ✨ Features

- 🔍 **Multi-source Aggregation Search**: Built-in dozens of free resource sites, one search returns all results
- 📄 **Rich Detail Pages**: Support for episode lists, actors, year, synopsis, and other complete information
- ▶️ **Smooth Online Playback**: Integrated HLS.js & ArtPlayer
- ❤️ **Favorites + Continue Watching**: Supports local storage, records viewing progress
- 📱 **PWA**: Offline cache, install to desktop/home screen, native mobile experience
- 🌗 **Responsive Layout**: Desktop sidebar + mobile bottom navigation, adapts to various screen sizes
- 🚀 **Simple Deployment**: One Docker command to run the complete service
- 👿 **Smart Ad Blocking**: Automatically skip slice ads in videos (experimental)

## 📋 Deployment Notes

This is the **No-Redis version**, using LocalStorage for user data storage. Suitable for personal or small-scale use.

### Features

- ✅ No additional database dependencies
- ✅ Simple and fast deployment
- ✅ Suitable for single-user use
- ⚠️ Data is stored locally in the browser; clearing browser data will lose records

## 🔒 Security Notice

**Important:** For your safety and to avoid potential legal risks:

- ✅ **Must Set Access Password**: A random password will be automatically generated during deployment
- ✅ **For Personal Use Only**: Do not publicly share or distribute your instance link
- ✅ **Comply with Local Laws**: Ensure your usage complies with local laws and regulations

### Important Disclaimer

- This project is for learning and personal use only
- Do not use the deployed instance for commercial purposes or public services
- Users are solely responsible for any legal issues arising from public sharing
- Project developers are not liable for users' usage behavior

## 📖 Usage Instructions

1. After deployment, access the Web interface
2. Enter the set access password to log in
3. Start searching and watching video content
4. Favorites and playback history will be automatically saved in the browser locally

## 🔗 Related Links

- GitHub: https://github.com/samqin123/MoonTV
- Tech Stack: Next.js 14 · Tailwind CSS 3 · TypeScript
- Player: ArtPlayer · HLS.js

## 📝 License

[MIT](https://github.com/samqin123/MoonTV/blob/main/LICENSE) © 2025 MoonTV & Contributors
