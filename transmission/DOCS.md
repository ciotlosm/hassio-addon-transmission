## Configuration

**Note**: _Remember to restart the add-on when the configuration is changed._

Transmission add-on configuration:

```json
{
  "log_level": "info",
  "authentication_required": false,
  "username": "",
  "password": "",
  "openvpn_enabled": false,
  "openvpn_config": "",
  "openvpn_username": "",
  "openvpn_password": ""
}
```

### Option: `log_level`

The `log_level` option controls the level of log output by the addon and can
be changed to be more or less verbose, which might be useful when you are
dealing with an unknown issue. Possible values are:

- `trace`: Show every detail, like all called internal functions.
- `debug`: Shows detailed debug information.
- `info`: Normal (usually) interesting events.
- `warning`: Exceptional occurrences that are not errors.
- `error`:  Runtime errors that do not require immediate action.
- `fatal`: Something went terribly wrong. Add-on becomes unusable.

Please note that each level automatically includes log messages from a
more severe level, e.g., `debug` also shows `info` messages. By default,
the `log_level` is set to `info`, which is the recommended setting unless
you are troubleshooting.

### Option: `authentication_required`

This option can be used to password protect the web-ui.

### Option: `username`

The username for authentication.

### Option: `password`

The password for authentication.

### Option: `openvpn_enabled`

Enable OpenVPN to anonymize your torrent activity.

### Option: `openvpn_config`

The name of .ovpn file. You should put it in `/config/openvpn`.

### Option: `openvpn_username`

Your OpenVPN username.

### Option: `openvpn_password`

Your OpenVPN password.
