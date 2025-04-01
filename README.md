# esphome-config
Contains common configuration settings for ESPHome devices that reference it via the `!include` directive.

See [ESPHome -- Remote Git Packages](https://esphome.io/components/packages.html#remote-git-packages) for more information.

## Usage
in your device yaml in ESPHome:
```
packages:
  # Simplify configuration by reusing common settings across all devices
  # https://github.com/dbensmith/esphome-config
  dbensmith.esphome-config:
    url: https://github.com/dbensmith/esphome-config
    files: [ common.yaml, uptime_sensor.yaml ]
    ref: main
    refresh: 0s
```
Select the files you want to include in the `files` property. In most cases, `common.yaml` is sufficient.
