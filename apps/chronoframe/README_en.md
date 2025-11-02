# ChronoFrame

A smooth photo display and management application, supporting multiple image formats and large-size image rendering.

## Features

### 🖼️ Powerful Photo Management

- **Manage photos online** - Easily manage and browse photos via the web interface
- **Explore map** - Browse photo locations on a map
- **Smart EXIF parsing** - Automatically extracts metadata such as capture time, geolocation, and camera parameters
- **Reverse geocoding** - Automatically identifies photo shooting locations
- **Multi-format support** - Supports mainstream formats including JPEG, PNG, HEIC/HEIF
- **Smart thumbnails** - Efficient thumbnail generation using ThumbHash

### 🔧 Modern Tech Stack

- **Nuxt 4** - Built on the latest Nuxt framework with SSR/SSG support
- **TypeScript** - Full type safety
- **TailwindCSS** - Modern CSS framework
- **Drizzle ORM** - Type-safe database ORM

### ☁️ Flexible Storage Solutions

- **Multiple storage backends** - Supports S3-compatible storage, local filesystem

## Getting Started

After the first deployment, please visit the web interface for initial setup.

By default, the application uses the built-in SQLite database. If you need to use another database (such as PostgreSQL), please configure the `DATABASE_URL` environment variable.

## Documentation

For more details, please visit the official documentation: https://chronoframe.bh8.ga/

## Links

- GitHub: https://github.com/HoshinoSuzumi/chronoframe
- Live Demo: https://lens.bh8.ga
