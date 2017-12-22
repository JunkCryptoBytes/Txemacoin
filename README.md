[![N|Solid](https://txemacoin.fr.to/txm_logo_m.png)](https://txemacoin.fr.to)
# Txemacoin
https://txemacoin.fr.to Copyright (c) 2009-2018 Bitcoin Developers Copyright (c) 2011-2018 Litecoin 
Developers What is Txemacoin? ---------------- Txemacoin is a lite version of Bitcoin using scrypt as a 
proof-of-work algorithm.
 - 2.5 minute block targets
 - subsidy halves in 840k blocks (~4 years)
 - ~84 million total coins The rest is the same as Bitcoin.
 - 50 coins per block
 - 2016 blocks to retarget difficulty For more information, as well as an immediately useable, binary version 
of the Txemacoin client sofware, see https://txemacoin.fr.to. License ------- Txemacoin is released under the 
terms of the MIT license. See `COPYING` for more information or see http://opensource.org/licenses/MIT.
# Installation
## Windows
#### Requirements and repository
```sh cd /mnt git clone https://github.com/JunkCryptoBytes/Txemacoin apt-get install \
    autoconf automake autopoint bash bison bzip2 cmake flex gettext \
    git g++ gperf intltool libffi-dev libgdk-pixbuf2.0-dev \
    libtool-bin libltdl-dev libssl-dev libxml-parser-perl make \
    openssl p7zip-full patch perl pkg-config python ruby scons \
    sed unzip wget xz-utils g++-multilib libc6-dev-i386 -y ```
#### Compile MXE
```sh git clone https://github.com/mxe/mxe.git cd /mnt/mxe make MXE_TARGETS="i686-w64-mingw32.static" boost 
make MXE_TARGETS="i686-w64-mingw32.static" qttools make MXE_TARGETS="i686-w64-mingw32.static" qt ```
#### Build Berkeley DB
```sh cd /mnt cp /mnt/Txemacoin/files/windows/db-4.8.30.tar.gz . tar zxvf db-4.8.30.tar.gz cd /mnt/db-4.8.30 
cp /mnt/Txemacoin/files/windows/compile-db.sh . ./compile-db.sh ```
#### Build MiniUPnP
```sh cd /mnt cp /mnt/Txemacoin/files/windows/miniupnpc-1.6.20120509.tar.gz . tar zxvf 
miniupnpc-1.6.20120509.tar.gz cd /mnt/miniupnpc-1.6.20120509 cp /mnt/Txemacoin/files/windows/compile-m.sh . 
./compile-m.sh ```
#### Build Txemacoin
```sh cd /mnt/Txemacoin cp /mnt/Txemacoin/files/windows/compile-txm.sh . ./compile-txm.sh ```
### Result:
```sh /mnt/Txemacoin/release/Txemacoin-qt.exe
```
