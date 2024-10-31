# FW-V03 branch
Customized specifically for XL2411P with FW V03 to facilitate overclocking.<br/>
Since FW version ~2 the ususal OpCode 0xDC is no longer effective after monitor exceeds its frequency range, and 0xCC now has to be adjusted after fixing black screen. This branch exist for the devices with FW versions prior to ~9.

## Launch parameters
3 parameters going in sequence:
```
<Pic delay> <OOR delay value to be summed with pic delay> <Wake delay>
```

Default:
```
2000 5000 3000
```