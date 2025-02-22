<div align="center">
   <a href="https://github.com/gitset-dev/gitset-desktop" target="_blank">
        <img src="https://github.com/imprvhub/gitset/blob/main/public/favicon-114-precomposed.png" alt="Gitset" />
    </a>
    <br>
    <a href="https://github.com/gitset-dev/gitset-desktop" target="_blank">
        <img src="https://img.shields.io/github/v/release/imprvhub/gitset-desktop?color=%237BFEF5" alt="version" />
    </a>
</div>

<div align="center">
    <h3>
        <a href="https://gitset.dev" target="_blank">
            GitSet Desktop - Cross-Platform Desktop Application
        </a>
    </h3>
</div>

<hr>

**GitSet Desktop** is the official cross-platform desktop application for [GitSet.dev](https://gitset.dev) - an advanced AI-driven GitHub tools suite. This electron-based application provides a dedicated desktop experience across macOS, Windows, and Linux systems, allowing users to access all GitSet features in a native application environment.

## Features

- **Cross-Platform Support**: Runs natively on macOS, Windows, and Linux
- **Seamless Integration**: Provides the complete GitSet.dev experience in a dedicated desktop environment
- **Custom Window Controls**: Platform-specific window controls for a native experience
- **Offline Capability**: Access to cached content even when offline
- **System Integration**: Native notifications and system tray integration

## Technical Architecture

GitSet Desktop is built with Electron, providing a consistent experience across all supported platforms while maintaining native OS integrations. The application wraps the GitSet.dev web application in a desktop environment, with custom window management and menu options.

```
├── main.js              # Main electron process
├── package.json         # Project configuration and dependencies
└── build/               # Build resources
    └── icons/           # Application icons for different platforms
```

## Installation

### Prerequisites

- Node.js (v16.x or later)
- npm (v7.x or later)

### Development Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/gitset-dev/gitset-desktop.git
   cd gitset-desktop
   ```


### Building Installers

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

## Technical Configuration

The application is configured to provide native-like experience on each platform:

### macOS
- Uses `hiddenInset` title bar style for a more integrated experience
- Includes standard macOS application menu structure
- Builds DMG installer

### Windows
- Uses custom application icon
- Includes standard application menus
- Builds NSIS installer

### Linux
- Supports AppImage and DEB package formats
- Includes standard menu structure
- Categorized as Development tool in application launchers

## Platform Compatibility

| Platform | Supported Versions                |
|----------|-----------------------------------|
| macOS    | 10.13 (Sierra) or later          |
| Windows  | Windows 10, Windows 11           |
| Linux    | Ubuntu 18.04+, Fedora 30+, etc.  |

## Versioning
GitSet Desktop maintains version parity with the web application, with both platforms sharing the same version numbers in most releases. This parallel versioning strategy is possible because the desktop application primarily serves as a wrapper for the web app with minimal platform-specific modifications. Any divergence in version numbers typically indicates desktop-specific enhancements or platform optimizations.

## Related Projects

- [GitSet](https://github.com/imprvhub/gitset) - The main GitSet.dev web application
- [GitSet CLI](https://github.com/gitset-dev/gitset-cli) - Command-line interface for GitSet services

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

For more information regarding licensing please read the [Terms and Conditions](https://gitset.dev/terms) on the GitSet website.
