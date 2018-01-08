# drmdecrypt
## Synopsis
This is a UNIX(c) Port of the DRMdecrypt i found somewhere on the net. It is capable of extracting the encryption key from the .mdb file and decrypts the .srf to a standard transport stream format.

Working but slooooowwww.

## Building

There is no Makefile at the moment. You will need a C-Compiler

* gcc -D_FILE_OFFSET_BITS=64 -D_LARGEFILE_SOURCE -D_LARGEFILE64_SOURCE -c aes.c -o aes.o
* gcc -D_FILE_OFFSET_BITS=64 -D_LARGEFILE_SOURCE -D_LARGEFILE64_SOURCE -c DRMDecrypt.c -o DRMDecrypt.o
* gcc -o drmdecrypt aes.o DRMDecrypt.o

## Blog

There is a [blog](http://ivo2u.nl/5e) post explaining the how for this piece of code

## Note

This project is NOT maintained anymore, but should still work. If you make changes and do a pull request I will merge them and give credit where credit is due, but I will not take change requests anymore.
