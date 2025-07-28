# Turso Plugin

Plugin for the [`turso`](https://www.nixhub.io/packages/turso-cli) package. This plugin sets several `TURSO` environment variables to run an instance of Turso in your local project.

## How to Activate

To install Turso, run `devbox add turso-cli@latest`

To activate this plugin, add the following reference to the `include` section of your `devbox.json` file.

```json

"include": [
    "github:captainseeker/devbox-plugins?dir=turso"
],
```

## Services

* turso

Use `devbox services up turso` to start the Turso  server

## Files

This plugin creates the following helper files:

* **.devbox/virtenv/turso/process-compose.yaml** - Defines the process to start the Turso server

## Environment Variables

This plugin sets the following environment variables:

* **TURSO_PORT** = 8080
* **TURSO_DB_FILE** = turso.db