# Afilmory

Afilmory (/əˈfɪlməri/, "uh-FIL-muh-ree") is a term created for personal photography websites, blending Auto Focus (AF), aperture (light control), film (vintage medium), and memory (captured moments).

A modern photo gallery website built with React + TypeScript, supporting automatic photo synchronization from multiple storage sources (S3, GitHub), featuring high-performance WebGL rendering, masonry layout, EXIF information display, thumbnail generation, and more.

## Features

### 🖼️ Core Functionality

- **High-Performance WebGL Image Renderer** - Custom WebGL component with smooth zoom and pan operations
- **Responsive Masonry Layout** - Powered by Masonic, adapts to different screen sizes
- **Modern UI Design** - Built with Tailwind CSS and Radix UI component library
- **Incremental Sync** - Smart change detection, processes only new or modified photos
- **i18n** - Multi-language support
- **OpenGraph** - OpenGraph metadata for social media sharing

### 📷 Image Processing

- **HEIC/HEIF Format Support** - Automatic conversion of Apple device HEIC format
- **TIFF Format Support** - Automatic conversion of TIFF format
- **Smart Thumbnail Generation** - Multi-size thumbnails for optimized loading performance
- **EXIF Information Display** - Complete shooting parameters including camera model, focal length, aperture, etc.
- **Blurhash Placeholders** - Elegant image loading experience
- **Live Photo Support** - Detection and display of iPhone Live Photos
- **HDR Image Support** - Display HDR images

### 🎛️ Advanced Features

- **Fujifilm Recipe** - Read and display Fujifilm camera film simulation settings
- **Fullscreen Viewer** - Image viewer with gesture support
- **File System Tags** - Auto-generated tags based on file system
- **Concurrent Processing** - Multi-process/multi-thread concurrent processing support
- **Multi-Storage Support** - S3, GitHub, and other storage backends
- **Share Image** - Share image to social media or embed iframe to your website
- **Interactive Map Explorer** - Geographic visualization of photos with GPS coordinates from EXIF data using MapLibre

## Getting Started

After deployment, you need to configure the storage backend (S3, GitHub, etc.) and set the corresponding environment variables.

After the first deployment, please visit the web interface for initial setup.

## Documentation

For more details, please visit the official documentation: https://docs.afilmory.art/

## Links

- Official Website: https://afilmory.art/
- GitHub: https://github.com/Afilmory/afilmory
- Documentation: https://docs.afilmory.art/
