# Opendate Claude Code Marketplace

Official plugin marketplace for the Opendate team and community.

## Installation

Add the marketplace to Claude Code:

```
/plugin marketplace add opendate-app/claude-marketplace
```

## Available Plugins

| Plugin | Description | Install |
|--------|-------------|---------|
| **ruby-lsp** | Ruby language intelligence (go-to-definition, references, hover) | `/plugin install ruby-lsp@opendate-marketplace` |
| **defect-product-areas** | Sort Linear issues into one Product Area using the team.opendate.io ownership page (Opendate staff; private repo) | `/plugin install defect-product-areas@opendate-marketplace` |

## Installing Plugins

Once the marketplace is added:

```
/plugin install <plugin-name>@opendate-marketplace
```

## For Contributors

### Adding a New Plugin

1. Create your plugin repo in the `opendate-app` org
2. Add an entry to `.claude-plugin/marketplace.json`
3. Submit a PR

### Plugin Entry Format

```json
{
  "name": "your-plugin",
  "source": {
    "source": "github",
    "repo": "opendate-app/your-plugin-repo"
  },
  "description": "Brief description",
  "version": "1.0.0",
  "author": {
    "name": "Your Name"
  },
  "license": "MIT",
  "keywords": ["tag1", "tag2"],
  "category": "languages|productivity|workflow|testing"
}
```

## Categories

- **languages** - Language servers and syntax support
- **productivity** - Workflow automation and efficiency tools
- **workflow** - Development process tools
- **testing** - Test runners and coverage tools

## License

MIT
