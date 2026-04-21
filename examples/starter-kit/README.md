/* TDK Starter Kit */

This is a minimal working example of a TDK-based project.

## Structure

```
my-service/
├── service.json          # Service manifest
├── src/
│   └── index.ts         # Entry point
├── package.json         # Dependencies
└── Tiltfile             # Local overrides
```

## Quick Start

1. Copy this directory
2. Update `service.json` with your service name
3. Run `tilt up`

## Files

### service.json

```json
{
  "appName": "my-service",
  "appType": "backend",
  "domain": "my-domain",
  "port": 4000
}
```
