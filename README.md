# Lemonade Desktop Snap

Desktop client for local AI chat powered by [lemonade-server](https://github.com/kenvandine/lemonade-server-snap).

Lemonade provides a clean, user-friendly chat interface for interacting with large language models (LLMs) running locally on your machine, with support for GPU and NPU acceleration.

## Requirements

This snap requires **lemonade-server** to be installed and running. The server provides the AI backend that powers this desktop client.

Install lemonade-server:

```bash
sudo snap install lemonade-server
```

The server starts automatically after installation. Verify it is running with:

```bash
snap services lemonade-server
```

The desktop client connects to lemonade-server on **localhost port 8000**.

## Installation

```bash
sudo snap install lemonade
```

## Features

- Modern chat interface for AI conversations
- Hardware-accelerated inference on GPUs and NPUs
- Runs entirely on your local machine for privacy
- Native Wayland and X11 support

## Building from Source

To build the snap locally:

```bash
snapcraft
```

Install the locally built snap:

```bash
sudo snap install lemonade_*.snap --dangerous
```

## Links

- [Lemonade SDK](https://github.com/lemonade-sdk/lemonade) - Upstream project
- [lemonade-server snap](https://github.com/kenvandine/lemonade-server-snap) - Required server component
- [Report Issues](https://github.com/kenvandine/lemonade-snap/issues)

## License

Apache-2.0
