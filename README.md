# Spotify Admute

> Disclaimer: This is just a proof of concept.

Hate spotify ads? this script _might_ help you.

## Dependencies

- [pulseaudio](https://man.archlinux.org/man/pactl.1.en)
- [playerctl](https://github.com/altdesktop/playerctl)

## Run as daemon

If you are running systemd, copy `systemd/admute.service` to `$HOME/.config/user/systemd/` then

```bash
# start service
systemctl --user start admute.service

# automatically run service on boot
systemctl --user enable admute.service
```

## Todo

- [x] write systemd service file
- [x] finish README
- [ ] measure performace

