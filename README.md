# OOR Buster XL2411P special
Customized specifically for XL2411P with FW V03 to facilitate overclocking.<br/>
Since FW version ~3 the ususal VCP feature code 0xDC is no longer effective after monitor exceeds its frequency range, and 0xCC now has to be adjusted after fixing black screen. This fork is aimed at fixing this.

## Launch parameters
3 parameters going in sequence (you can create a shortcut to `OorBuster.exe` and add these in _Target_ field):
```
<Pic delay> <OOR delay value to be summed with pic delay> <Wake delay>
```

Default:
```
2000 5000 3000
```

### To launch with Windows (important if you keep overclock at all times):
Put the .exe (or shortcut if using custom launch parameters) into
```
%ProgramData%\Microsoft\Windows\Start Menu\Programs\StartUp
```

## Compared to the original
* Removed AMA Mode restoration feature
* Introduced new OOR workaround and removed old one
* Reworked the APP menu a bit
* Changed the icon 

### Status
| XL2411P FW Version | FW Binaries ([confirmed working](https://youtu.be/44rDRHatMKI?si=d5ABKtteKY3Da8i4))              | The app fixes black screen                 | The app removes OOR notification          |
|:-------------------|:-------------------------------------------------------------------------------------------------|:-------------------------------------------|:------------------------------------------|
| V02                |❔                                                                                                |❔                                          |❔                                          |
| V03                |[Download](https://github.com/Maxinator500/OOR-Buster-XL2411P-special/blob/files/XL2411P-FW03.bin)|✅                                         |✅                                         |
| V06                |❔                                                                                                |❔                                          |❔                                          |
| V09                |[Download](https://github.com/Maxinator500/OOR-Buster-XL2411P-special/blob/files/XL2411P-FW09.bin)|✅                                         |❌                                         |
| V10                |[Download](https://github.com/Maxinator500/OOR-Buster-XL2411P-special/blob/files/XL2411P-FW10.bin)|✅                                         |❌                                         |
| V13                |[Download](https://github.com/Maxinator500/OOR-Buster-XL2411P-special/blob/files/XL2411P-FW13.bin)|✅                                         |❌                                         |
