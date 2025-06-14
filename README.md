<div align="center">
   <a href="https://github.com/gitset-dev/gitset-desktop" target="_blank">
        <img src="https://github.com/imprvhub/gitset/blob/main/public/favicon-114-precomposed.png" alt="Gitset" />
    </a>
    <br>
    <a href="https://github.com/gitset-dev/gitset-desktop" target="_blank">
        <img src="https://img.shields.io/static/v1?label=version&message=v1.9.0&color=7BFEF5" alt="version" />
    </a>
</div>

<div align="center">
    <h3>
        <a href="https://gitset.dev" target="_blank">
            Gitset Desktop - Cross-Platform Desktop Application
        </a>
    </h3>
</div>

<hr>

**Gitset Desktop** is the official cross-platform desktop application for [Gitset.dev](https://gitset.dev) - an advanced AI-driven GitHub tools suite. This Electron-based application provides a dedicated desktop experience across macOS, Windows, and Linux systems, allowing users to access all Gitset features in a native application environment with seamless token synchronization.

### Features

- **Cross-Platform Support**: Runs natively on macOS, Windows, and Linux
- **Seamless Integration**: Provides the complete Gitset.dev experience in a dedicated desktop environment
- **Native Window Controls**: Platform-specific window controls with proper drag and resize functionality
- **Shared Token System**: Synchronized token usage with the web application across all platforms
- **System Integration**: Native notifications and platform-optimized interface

### Technical Architecture

Gitset Desktop is built with Electron, providing a consistent experience across all supported platforms while maintaining native OS integrations. The application wraps the Gitset.dev web application in a desktop environment with optimized performance.

```
├── main.js              # Main electron process
├── package.json         # Project configuration and dependencies
└── build/               # Build resources
    └── icons/           # Application icons for different platforms
```

### Installation

#### Prerequisites

- Node.js (v16.x or later)
- npm (v7.x or later)

#### Development Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/gitset-dev/gitset-desktop.git
   cd gitset-desktop
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

#### Building Installers

To build installers for all supported platforms:

```bash
npm run build
```

For platform-specific builds:

```bash
npm run build:mac    # For macOS
npm run build:win    # For Windows
npm run build:linux  # For Linux
```

### Platform Configuration

The application is configured to provide native-like experience on each platform:

#### macOS
- Native title bar with proper drag functionality
- Standard macOS application menu structure
- Builds DMG installer

#### Windows
- Custom application icon and window controls
- Standard application menus
- Builds NSIS installer

#### Linux
- Supports AppImage and DEB package formats
- Standard menu structure
- Categorized as Development tool in application launchers

### Platform Compatibility

| Platform | Supported Versions                |
|----------|-----------------------------------|
| macOS    | 10.13 (Sierra) or later          |
| Windows  | Windows 10, Windows 11           |
| Linux    | Ubuntu 18.04+, Fedora 30+, etc.  |

### Versioning Strategy

Gitset Desktop maintains version parity with the web application, ensuring feature consistency across platforms. The desktop application serves as a native wrapper for the web platform with optimized window management and system integration. Version updates are released concurrently to maintain synchronized functionality and token system compatibility.

### Related Projects

- [Gitset](https://github.com/imprvhub/gitset) - The main Gitset.dev web application
- [Gitset MCP Agent](https://github.com/gitset-dev/gitset-mcp) - Model Context Protocol agent for terminal and IDE integration (in development)

### Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### License

For more information regarding licensing please read the [Terms and Conditions](https://gitset.dev/terms) on the Gitset website.