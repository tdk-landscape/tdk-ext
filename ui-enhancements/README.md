# UI Enhancements Extension

Injects CSS and JavaScript into Tilt web UI for improved UX.

## Features

- **Tooltips**: Hover tooltips on resources explaining their purpose
- **Icons**: Status icons for better visual scanning
- **Help Panel**: Side panel with documentation and shortcuts
- **Cron Jobs Tab**: Dedicated tab for monitoring cron jobs

## Installation

Add to your Tiltfile:

```starlark
load("ext://github.com/tdk-landscape/tdk-ext/ui-enhancements", "load_ui_enhancements")

load_ui_enhancements()
```

## Configuration

```starlark
load_ui_enhancements({
    "enable_tooltips": True,        # Resource hover tooltips
    "enable_icons": True,           # Status icons
    "enable_help_panel": True,      # Help side panel
    "enable_cron_jobs_tab": True    # Cron jobs monitoring
})
```

## Server

The extension runs an HTTP server on port 10351 serving:
- `/ui-enhancements.css` - Combined CSS
- `/ui-enhancements.js` - Combined JavaScript
