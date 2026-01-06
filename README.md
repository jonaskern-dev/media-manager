# Media Manager

Media automation platform with Save.tv integration, download management, and Plex-compatible file organization.

## Installation

### Homebrew (macOS/Linux)

```bash
brew tap jonaskern-dev/tap
brew install media-manager
```

### Binary Download

Download the latest release for your platform from the [Releases](https://github.com/jonaskern-dev/media-manager/releases) page:

| Platform | Architecture | Binary |
|----------|-------------|--------|
| macOS | Apple Silicon (M1/M2/M3) | `media-manager-darwin-arm64` |
| macOS | Intel | `media-manager-darwin-amd64` |
| Linux | x86_64 | `media-manager-linux-amd64` |
| Linux | ARM64 | `media-manager-linux-arm64` |

```bash
# Example: Download and install on macOS ARM
curl -L https://github.com/jonaskern-dev/media-manager/releases/latest/download/media-manager-darwin-arm64 -o media-manager
chmod +x media-manager
sudo mv media-manager /usr/local/bin/
```

### Docker

```bash
docker pull registry.itksrv.de/jonas/media-manager:latest
```

## Usage

```bash
# Show version
media-manager --version

# Start server
media-manager server

# Show help
media-manager --help
```

## Features

- Save.tv API integration (recordings, downloads)
- Duplicate detection (fuzzy matching for movies, S/E for series)
- Plex-compatible file structure
- Concurrent download workers
- REST API
- Web UI (planned)

## License

MIT
