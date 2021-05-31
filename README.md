# systemd

[![Build Status](https://drone.osshelp.ru/api/badges/ansible/systemd/status.svg)](https://drone.osshelp.ru/ansible/systemd)

Role for managing systemd parameters

## Usage (example)

```yaml
    - role: systemd
      systemd_target_server_type: physical
      systemd_custom_params:
        - { key: param1, value: 'yes' }
        - { key: param2, value: 'no' }
```

## Available parameters

### Main

| Param | Default | Description |
| -------- | -------- | -------- |
| `systemd_setup` | `full` | Setup mode. See [OSSHelp KB article](https://oss.help/kb4895) |
| `systemd_target_server_type` | `-` | Target server type (physical or virtual) |
| `systemd_skip_services` | `[]` | List of services to skip |
| `systemd_custom_params` | `[]` | List of custom params for `/etc/systemd/systemd.conf` |

## FAQ

...

## Useful links

...

## TODO

...

## License

GPL3

## Author

OSSHelp Team, see <https://oss.help>
