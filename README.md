# esphome-config
Contains common configuration settings for ESPHome devices that reference it via the `!include` directive.

See [ESPHome -- Remote Git Packages](https://esphome.io/components/packages.html#remote-git-packages) for more information.

## Usage
in your device yaml in ESPHome:
```
packages:
  # Simplify configuration by reusing common settings across all devices
  # https://github.com/dbensmith/esphome-config/blob/main/common.yaml
  dbensmith.common:
    url: https://github.com/dbensmith/esphome-config
    files: common.yaml
    ref: main
    refresh: 0s
```
