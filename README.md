# Devbox Plugins

This repository includes plugins for configuring packages using Devbox.

## Available Plugins

* [Valkey](./valkey)

## How to Use

Each subfolder contains a plugin for a specific package. To use a plugin, add the following reference to the `include` section of your `devbox.json` file.

```json
"include": [
    "github:captainseeker/devbox-plugins?dir=<plugin-name>"
],
```