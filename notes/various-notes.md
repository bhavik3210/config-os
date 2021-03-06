### Standard Notes (Theme Config)

org.standardnotes.theme-focus
/home/bhavik/.config/Standard Notes/Extensions/org.standardnotes.theme-focus
replace **a464c2** with **313131**

### Give Virtual Box Users access to USB

sudo adduser \$USERNAME vboxusers

### GTK3 Themes

headerbar.default-decoration to change titlebar

```
3b3b3b to 1e1e1e
373737 to 222222
updated: 222222 to 1a1a1a
```

navbar to change menubar

css id/class/groups
popup-menu (to change colors of dropdown windows in gnome panel) (in gnome-shell.css)

#### Menu Bar

```
menubar,
.menubar {
  -GtkWidget-window-dragging: true;
  padding: 0px;
  background-color: #242424;
  background-image: none;
  color: rgba(225, 219, 219, 0.8);
  box-shadow: inset 0 -1px rgba(255, 255, 255, 0.12);
}
```

### TO CHANGE LOCK SCREEN

cd into /usr/share/gnome-shell/theme
file ubuntu.css or pop.css

#lockDialogGroup {
background: #1a1a1a url(resource:///org/gnome/shell/theme/noise-texture.png);
background-repeat: repeat;
}

```

### Change DNS lookup on ubuntu

sudo nano /etc/resolv.conf

remove existing

```

nameserver x.x.x.x

```

replace with your dns primary and secondary

```

nameserver x.x.x.x
nameserver x.x.x.x

```

restart machine

### Change Wifi Power savings

cd /etc/NetworkManager/conf.d/
nano default-wifi-powersave-on.conf

change value for wifi.powersave = x

```

0 (use default), 1 (ignore/don't touch), 2 (disable) or 3 (enable).
wifi.powersave = 2

```

Change wifi.powersave to 2 to disable it

Highlight Color: #545454

### Flameshot Shortcuts

- Entire Screensshot

  - Shift + Ctrl + 3
  - `flameshot full -p /home/bhavik/Pictures/Screenshots`

- Portion of Screenshot

  - Shift + Ctrl + 4
  - `flameshot gui -p /home/bhavik/Pictures/Screenshots`

### Watch settings change commands

`dconf watch /`
```
