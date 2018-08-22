# CropCoin
CropCoin is an Asic resistant,Community Focused,Secure and Decentralized Cryptocurrency.
Pow phase will start on 02 February, 2018 at 11:00 UTC.

## How to build the wallet (ubuntu 16.04)
```
sudo su
apt-get update
apt -y install software-properties-common
apt-add-repository -y ppa:bitcoin/bitcoin
apt-get update
apt install -y make build-essential libtool software-properties-common autoconf \
    libssl-dev libboost-dev libboost-chrono-dev libboost-filesystem-dev \
    libboost-program-options-dev libboost-system-dev libboost-test-dev \
    libboost-thread-dev sudo automake git pwgen libdb4.8-dev \
    bsdmainutils libdb4.8++-dev libminiupnpc-dev libgmp3-dev

git clone https://github.com/Cropdev/CropDev.git
cd CropDev/src
mkdir obj/support
mkdir obj/crypto
make -j$(nproc) -f makefile.unix
cp cropcoind /usr/local/bin
```
