# st - Terminal Emulator from Suckless

The `config.def.h` is default configuration from st distribution. Just copy this to `config.h` if you don't want to change anything. If you want to change anything, copy to `config.h` then edit. The [config.h](config.h) file here is my configuration. I change the font size and background color:

```bash
$ diff config.def.h config.h
8c8
< static char *font = "Liberation Mono:pixelsize=12:antialias=true:autohint=true";
---
> static char *font = "Liberation Mono:pixelsize=20:antialias=true:autohint=true";
123,124c123,124
<       "gray90", /* default foreground colour */
<       "black", /* default background colour */
---
>   "#2f2c45",
>   "#928FB0",
132,133c132,133
< unsigned int defaultfg = 258;
< unsigned int defaultbg = 259;
---
> unsigned int defaultfg = 259;
> unsigned int defaultbg = 258;
```

Taken from [Original AUR package](https://aur.archlinux.org/packages/st)
