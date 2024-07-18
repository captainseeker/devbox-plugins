# Valkey Plugin

Plugin for the [`valkey`](https://www.nixhub.io/packages/valkey) package. This plugin sets several `VALKEY` environment variables to run an instance of Valkey in your local project, adds a `valkey.conf` file to the devbox.d directory, and configures a valkey service.

## How to Activate

To install Valkey, run `devbox add valkey@latest`

To activate this plugin, add the following reference to the `include` section of your `devbox.json` file.

```json

"include": [
    "github:captainseeker/devbox-plugins?dir=valkey"
],
```

## Services

* valkey

Use `devbox services up valkey` to start the Valkey  server

## Files

This plugin creates the following helper files:

* **devbox.d/valkey/valkey.conf** - Valkey configuration file
* **.devbox/virtenv/valkey/process-compose.yaml** - Defines the process to start the Valkey server

## Environment Variables

This plugin sets the following environment variables:

* **VALKEY_PORT** = 6379
* **VALKEY_CONF** = {{.DevboxDir}}/valkey/valkey.conf