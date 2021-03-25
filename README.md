Current firmware for Sonos devices as of 2021-03-25. Described as:

```
Sonos OS: S2
Version: 13.0 (build 62186220)
```

Name: `62.1-86220-1-32.upd`.

This is the image downloaded by the device from Sonos, so it will consume the whole image.

The first 320 bytes of the image in hex:

```
49 7F 16 35 01 00 00 00 1C 00 00 00 00 00 00 00 3E 00 00 00 01 00 00 00 CC 50 01 00 49 7F 16 35
02 00 00 00 2C 00 00 00 00 00 00 00 01 00 00 00 20 00 00 00 01 00 00 00 01 00 00 00 00 00 00 00
FE FF FF FF FF FF FF FF 49 7F 16 35 02 00 00 00 94 00 00 00 00 00 00 00 FD FF FF FF 02 00 00 00
00 00 00 00 00 00 00 00 04 00 00 00 02 00 00 00 22 00 00 00 07 00 00 00 DE 81 00 00 10 00 00 00
02 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 49 7F 16 35
02 00 00 00 2C 00 00 00 00 00 00 00 FE FF FF FF 00 00 00 00 00 00 00 00 FE FF FF FF 00 00 00 00
FE FF FF FF FF FF FF FF 49 7F 16 35 03 00 00 00 4A 15 00 00 04 00 00 00 88 64 99 CA 00 00 01 3A
00 01 00 00 00 00 00 00 01 00 00 00 14 03 8E 78 AF 62 01 F2 55 86 CB 8B 60 5E 67 7F 44 08 0A 83
```

The interesting pattern is: `49 7F 16 35` with 9 instances occuring in this image. 

There is also one instance of: `49 7F 16 AE` at offset `12896712` / `0xC4C9C8`

Binwalk is not much assistance. 