# pinecoin-PNE A Coin Backed by A Business.

https://pinecoin.org


pinecoin-PNE will become attached to Te Lion and shall proceed to become a very stable and viable option for Payments and Assets Alike we see this not only as a financial gain but also a greater means of publicizing crypto coins altogether to show what really is Possible.

In the Last 10 years there has been an enormous rate of growth within Crypto related working whether it be a source code to your secret projects I’m sure all has benefited since Crypto Coins have arisen. We are going to take Advantage of this and help pinecoin-PNE stand out more so.

We aim to achieve a foothold into Cryptography and the coins associated with it as we see the Importance in this and making them become more of a reality, The technology around the blockchain to which pinecoin-PNE is based is substantial to say the least. It has a source code that is usable and friendly but also Secure.



UNIX BUILD NOTES
====================

To Build pinecoin Headless 
-----------------

sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils

sudo apt-get install qt5-default qt5-qmake qtbase5-dev-tools qttools5-dev-tools build-essential libboost-dev libboost-system-dev libboost-filesystem-dev libboost-program-options-dev libboost-thread-dev libssl-dev libdb++-dev libminiupnpc-dev 

sudo apt-get install software-properties-common

sudo add-apt-repository ppa:bitcoin/bitcoin

sudo apt-get update

sudo apt-get install libdb4.8-dev libdb4.8++-dev

sudo apt-get install libqrencode-dev

git clone https://github.com/pinecoinPNE/pinecoin.git

cd pinecoin/src/secp256k1

chmod +x autogen.sh

sudo ./autogen.sh

sudo ./configure

sudo make && make install

cd

cd pinecoin/src/leveldb

sudo sh build_detect_platform build_config.mk .

cd

cd pinecoin/src

sudo make -f makefile.unix

strip pinecoind

LD_LIBRARY_PATH=/usr/local/lib

export LD_LIBRARY_PATH


To Build pinecoin-PNE Qt Wallet
------------------

sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils

sudo apt-get install qt5-default qt5-qmake qtbase5-dev-tools qttools5-dev-tools build-essential libboost-dev libboost-system-dev libboost-filesystem-dev libboost-program-options-dev libboost-thread-dev libssl-dev libdb++-dev libminiupnpc-dev 

sudo apt-get install software-properties-common
sudo add-apt-repository ppa:bitcoin/bitcoin
sudo apt-get update
sudo apt-get install libdb4.8-dev libdb4.8++-dev

sudo apt-get install libqrencode-dev

git clone https://github.com/pinecoinPNE/pinecoin.git

cd pinecoin/src/secp256k1

chmod +x autogen.sh

sudo ./autogen.sh

sudo ./configure

sudo make && make install

cd

cd pinecoin/src/leveldb

sudo sh build_detect_platform build_config.mk .

cd

cd pinecoin

sudo qmake pinecoin-PNE.pro

sudo make -jnumofcoreshere