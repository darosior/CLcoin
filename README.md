# CLcoin

CLcoin is a fork from Litecoin, with modified parameters. Created in order to use it to teach the use of cryptocurrencies to beginners.
http://www.crypto-lyon.fr
  
   
## Dependencies
Dependencies [from Bitcoin](https://github.com/bitcoin/bitcoin/blob/master/doc/dependencies.md)
Litecoin dependencies for [unix](https://github.com/litecoin-project/litecoin/blob/0.8/doc/build-unix.md), [OSX](https://github.com/litecoin-project/litecoin/blob/0.8/doc/build-osx.md), [Windows](https://github.com/litecoin-project/litecoin/blob/0.8/doc/build-msw.md)  
Other missing packets I noticed during the installation on a fresh install (Debain 9)
```
apt upgrade
apt update
apt install 
```

## Installation
```
git clone http://github.com/darosior/CLcoin && cd CLcoin/src
make -f makefile.unix USE_UPNP=-
cd ..
#GUI part
qmake USE_UPNP=-
make USE_UPNP=-
./CLcoind #Or ./CLcoin-qt for GUI
```

#### Note about compiling on linux
Many compilation problems come from bad version of libboost, libssl, or libdb4.8 (source can be found [here](https://launchpad.net/~bitcoin/+archive/ubuntu/bitcoin))
