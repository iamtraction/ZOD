# Zip of Death (ZOD)
This is a decompression bomb (also known as zip of death or zip bomb) designed t
o crash or render useless the program or system reading it.

It is usually a small file for ease of transport and to avoid suspicion.
However, when the file is unpacked, its contents are more than the system can
handle. It is often employed to disable antivirus software, in order to create
an opening for more traditional viruses.

Rather than hijacking the normal operation of the program, a zip bomb allows the
program to work as intended, but the archive is carefully crafted so that
unpacking it (e.g. by a virus scanner in order to scan for viruses) requires
inordinate amounts of time, disk space or memory.

*Most modern antivirus programs can detect whether a file is a zip bomb, to
avoid unpacking it.*

### `42.zip`
This repository contains the `42.zip` zip bomb, which is a zip file consisting
of 42 kilobytes of compressed data, containing five layers of nested zip files
in sets of 16, each bottom layer archive containing a 4.3 gigabyte
(4 294 967 295 bytes; ~ 3.99 GiB) file for a total of 4.5 petabytes
(4 503 599 626 321 920 bytes; ~ 3.99 PiB) of uncompressed data.

So, if you extract all the files, you will most likely run out of space.

```
16 x       4 294 967 295 bytes =        68 719 476 720 bytes ( 68.7 GB)
16 x      68 719 476 720 bytes =     1 099 511 627 520 bytes (  1.1 TB)
16 x   1 099 511 627 520 bytes =    17 592 186 040 320 bytes ( 17.6 TB)
16 x  17 592 186 040 320 bytes =   281 474 976 645 120 bytes (281.5 TB)
16 x 281 474 976 645 120 bytes = 4 503 599 626 321 920 bytes (  4.5 PB)
```

#### Password
`42`
