# Spotify Admute

Hate spotify ads? this script may help you.

## Dependencies

- [pactl](https://man.archlinux.org/man/pactl.1.en)
- [playerctl](https://github.com/altdesktop/playerctl)

## Run as daemon

If you are running systemd, 

1. copy `systemd/admute.service` to `$HOME/.config/user/systemd/`
2. edit the `ExecStart` path to `%h/path/to/script` (`%h` expands to `$HOME`), then

```bash
# start service
systemctl --user start admute.service

# automatically run service on boot
systemctl --user enable admute.service
```

If you're on i3wm, it is easier to just append this to your config,

```bash
exec --no-startup-id /path/to/script
```

## Todo

- [x] write systemd service file
- [x] finish README
- [ ] measure performace

