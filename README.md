# TDK Extensions

UI enhancements, IDE components, examples, and documentation for TDK Landscape.

## Purpose

Provides the developer experience layer:
- UI enhancements for Tilt (tooltips, icons, cron jobs tab, help panel)
- IDE components (file browser, code viewer, config inspector, terminal)
- Example services and starter kits
- Documentation

## Directory Structure

```
ui-enhancements/
├── tiltfile.py              # Main extension entry point
└── ui/
    ├── tooltips.{css,js}    # Contextual tooltips
    ├── icons.{css,js}       # Status icons
    ├── help-panel.{css,js}  # Help side panel
    └── cron-jobs-tab.{css,js} # Cron jobs monitoring

ide-components/
├── file-browser/          # Browse filesystem in browser
├── code-viewer/           # View source with syntax highlighting
├── config-inspector/      # Compare/edit master configs
└── code-executor/         # Run bun commands from browser

examples/
└── starter-kit/           # Minimal working TDK project

docs/
├── getting-started.md
├── architecture.md
└── api-reference.md
```

## Usage

### UI Enhancements

```starlark
load("ext://github.com/tdk-landscape/tdk-ext/ui-enhancements", "load_ui_enhancements")

load_ui_enhancements({
    "enable_tooltips": True,
    "enable_icons": True,
    "enable_help_panel": True,
    "enable_cron_jobs_tab": True
})
```

### IDE Components

Access via Traefik URLs:
- File Browser: http://files.localhost (port 9765)
- Code Viewer: http://viewer.localhost (port 9766)
- Config Inspector: http://configs.localhost (port 9767)
- Terminal: http://terminal.localhost (port 9768)

## License

MIT
