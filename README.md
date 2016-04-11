Clp compiled with sources from

http://www.stats.ox.ac.uk/pub/Rtools/goodies/sources/Clp-1.16.9.tar.xz

The 32- and 64-bit versions are made separately in Clp32 and Clp64
directories. This replicates the legacy layout used for Clp.

Compilation was performed by the following for 64 bit

```bash
./configure --enable-static --disable-shared --prefix=.../Clp32 --build=i686-w64-mingw32 && make && make install
```

```bash
./configure --enable-static --disable-shared --prefix=.../Clp64 --build=x86_64-w64-mingw32 && make && make install
```

To install pcaL1 set `CLP_PATH` to the location you extracted the zipfile.
