# drmdecrypt

NOTE: This project is probably deprecated. I don't expect it to work anymore on modern Samsung TV's.  

## Synopsis
This is a UNIX(c) Port of the DRMdecrypt i found somewhere on the net. It is capable of extracting the encryption key from the .mdb file and decrypts the .srf to a standard transport stream format.

Working but slooooowwww.

## Building

There is no Makefile at the moment. You will need a C-Compiler

* gcc -D_FILE_OFFSET_BITS=64 -D_LARGEFILE_SOURCE -D_LARGEFILE64_SOURCE -c aes.c -o aes.o
* gcc -D_FILE_OFFSET_BITS=64 -D_LARGEFILE_SOURCE -D_LARGEFILE64_SOURCE -c DRMDecrypt.c -o DRMDecrypt.o
* gcc -o drmdecrypt aes.o DRMDecrypt.o


# License - DWTFYWT

          DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                   Version 2, December 2004
 
Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>

Everyone is permitted to copy and distribute verbatim or modified
copies of this license document, and changing it is allowed as long
as the name is changed.
 
           DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
  TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

 0. You just DO WHAT THE FUCK YOU WANT TO.
