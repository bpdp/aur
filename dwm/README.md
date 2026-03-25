# dwm - Suckless dwm Window Manager

Change [config.h](config.h) file if you want to configure anything. Here's the diff between my package and upstream:

```bash
$ diff dwm/config.h dwm-6.8-orig/config.def.h
31c31
<       { "Firefox",  NULL,       NULL,       0,            0,           -1 },
---
>       { "Firefox",  NULL,       NULL,       1 << 8,       0,           -1 },
```

Using original configuration (`1 << 8`) makes Firefox always run in workspace 9.

Taken and modified from [original AUR package for dwm](https://aur.archlinux.org/packages/dwm)
