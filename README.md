# Nomana Notion Tools

A self-hosted web application that provides a rich interface on top of your Notion workspace — live dashboards, in-app editing, AI document analysis, Google Calendar sync, email sharing, PDF export, and role-based access control.

> **Source code** is maintained in a private repository. This repo hosts releases, documentation, issues, and discussions.

---

## Features

| Feature | Plan |
|---------|------|
| Dashboard with Kanban & table views | Community |
| In-app Notion page editing | Community |
| Role-based access control (RBAC) | Community |
| Custom icon library | Community |
| Full-text document indexing & search | Community |
| Google Calendar ↔ Notion sync | Plus |
| Email sharing of pages | Plus |
| PDF export | Plus |
| AI document analysis (Claude) | Pro |
| AI meeting transcription & summary | Pro |
| Semantic document search | Pro |

---

## Installation

### Docker (recommended)

```bash
docker pull ghcr.io/fblettner/nomana-notion:latest

docker run -d \
  --name nomana-notion \
  -p 8200:8200 \
  -v $(pwd)/data:/app/data \
  ghcr.io/fblettner/nomana-notion:latest
```

Then open `http://localhost:8200` in your browser.

See [docs/installation.md](docs/installation.md) for full Docker Compose setup.

### Desktop App

Download the latest release for your platform:

| Platform | Download |
|----------|----------|
| macOS (Apple Silicon / Intel) | `Nomana Notion-macOS.zip` |
| Windows | `Nomana Notion-Windows.zip` |

See [docs/installation.md](docs/installation.md) for installation steps.

### Python Package

```bash
pip install nomana-notion
nomana-start
```

---

## Quick Start

1. **Start the app** via Docker or desktop
2. **Log in** with the default credentials: `admin` / `admin` — change immediately in Settings → Users
3. **Configure Notion** in Settings → Notion: paste your [Notion integration token](https://www.notion.so/my-integrations)
4. **Enable databases** in Settings → Databases: connect your Notion databases

See [docs/configuration.md](docs/configuration.md) for detailed setup.

---

## Documentation

- [Installation Guide](docs/installation.md)
- [Configuration](docs/configuration.md)
- [Features Overview](docs/features.md)
- [API Reference](docs/api-reference.md)

---

## Issues & Discussions

- **Bug reports / feature requests**: [GitHub Issues](../../issues)
- **Questions / ideas**: [GitHub Discussions](../../discussions)

---

## License

MIT — by [nomana-it](https://nomana-it.fr)
