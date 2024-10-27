# OOR Buster XL2411P special
Customized specifically for XL2411P with FW V13 to facilitate overclocking.<br/>
Since FW version ~9 the ususal OpCodes 0xCC and 0xDC are no longer effective after monitor exceeds its frequency range. This fork is aimed at fixing this.

## Details
Manipulates manufacturer OpCode 0xEF (removes Out of Range notification from screen) and Overscan Mode 0xDA (fixes black screen) after hitting over 144Hz on your BenQ 144Hz monitor. The OpCodes are cached upon launching the app, so if you changed Overscan Mode while the app is running (e.g. from Normal to Overscan) and wish to use it, before switching to overclocked refresh rate right click the OOR Buster icon in tray and hit reload.

## Launch parameters
3 parameters going in sequence (you can create a shortcut to `OorBuster.exe` and add these in _Target_ field):
```
<OOR delay> <Pic delay value to be summed with OOR delay> <Wake delay>
```
- OOR delay - after something changes with the screen (refresh rate, fullscreen exclusive, etc.), wait this long before removing Out of Range notification;
- Pic delay - after OOR removal, wait this long before fixing black screen (not all monitors get black screen);
- Wake delay - after screen wakes up (after screen sleep or system sleep), wait this long before busting OOR again.

Default:
```
2000 500 3000
```

### To launch with Windows (important if you keep overclock at all times):
Put the .exe (or shortcut if using custom launch parameters) into
```
%ProgramData%\Microsoft\Windows\Start Menu\Programs\StartUp
```

## Compared to the original
* Removed AMA Mode restoration feature
* Introduced [new OOR workaround](https://forums.blurbusters.com/viewtopic.php?f=8&p=98852#p99028) and removed old one
* Reworked the APP menu a bit
* Changed the icon 

### Status
| XL2411P FW Version | FW Binaries ([confirmed working](https://youtu.be/44rDRHatMKI?si=d5ABKtteKY3Da8i4))           | The app fixes black screen | The app removes OOR notification |
|:-------------------|:----------------------------------------------------------------------------------------------|:---------------------------|:---------------------------------|
| V9                 |[Download](https://github.com/Maxinator500/OOR-Buster-XL2411P-special/blob/FW/XL2411P-FW09.bin)|✅                          |❌                       |
| V10                |[Download](https://github.com/Maxinator500/OOR-Buster-XL2411P-special/blob/FW/XL2411P-FW10.bin)|✅                          |❌                       |
| V13                |❔                                                                                             |❔                           |❔                        |
