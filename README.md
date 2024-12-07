# FW-V13 branch
Customized specifically for XL2411P with FW V13 to facilitate overclocking.<br/>
Since FW version ~6 the ususal VCP feature codes 0xCC and 0xDC are no longer effective after monitor exceeds its frequency range. This branch is the failed attempt to reproduce [the OOR workaround](https://forums.blurbusters.com/viewtopic.php?f=8&p=98852#p99028).

## Details
Manipulates manufacturer OpCode 0xEF (~~removes Out of Range notification from screen~~) and Overscan Mode 0xDA (fixes black screen) after hitting over 144Hz on your BenQ monitor.

## Alternative versions
Releases from other branches:<br/>FW-V03 - [Nov 1, 2024 release](https://github.com/Maxinator500/OOR-Buster-XL2411P-special/releases/tag/1.4-branchV03)

## Launch parameters
```
<OOR delay> <Pic delay> <Wake delay>
```

Default:
```
2000 500 3000
```
