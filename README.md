# gtklock-powerbar-module
gtklock module adding power controls to the lockscreen.

## Configuration
The configuration is done through the gtklock config file, in the `powerbar` section.

This is an example showing default settings:
```ini
[main]
modules=powerbar-module.so

[powerbar]
show-labels=false
linked-buttons=false
reboot-command=systemctl reboot
poweroff-command=systemctl -i poweroff
suspend-command=systemctl suspend
userswitch-command=
logout-command=
button-timeout=500
```

## About
Adds a reboot and poweroff button the the lockscreen.
The `gtklock-module.h` header can be used when making your own modules.

__⚠️ Module version matches the compatible gtklock version. Other versions might or might not work.__

## Dependencies
- Meson (build-time)
- pkg-config (build-time)
- gtk+3.0
