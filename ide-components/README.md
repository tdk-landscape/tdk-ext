# IDE Components

Web-based IDE components integrated into Tilt development environment.

## Components

| Component | Port | URL | Purpose |
|-----------|------|-----|---------|
| File Browser | 9765 | http://files.localhost | Browse filesystem |
| Code Viewer | 9766 | http://viewer.localhost | View source files |
| Config Inspector | 9767 | http://configs.localhost | Compare/edit configs |
| Code Executor | 9768 | http://terminal.localhost | Run bun commands |

## Technology

All components are Python HTTP servers (zero additional dependencies):
- Works even if Bun/Node has issues
- No build step required
- Python is pre-installed

## Installation

Add to your Tiltfile:

```starlark
load("ext://github.com/tdk-landscape/tdk-ext/ide-components", "load_ide_components")

load_ide_components()
```
