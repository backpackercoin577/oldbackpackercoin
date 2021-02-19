Backpackercoin 
====================
                            
* Ticker: BPC  
* Consensus: Hybrid PoW/PoS 
* Algorithm:X15
* Peer to Peer Port: 21320
* RPC Port: 22320
* Last POW Block: 20000
* Mininum Stake Age: One Hour
* Maximum Stake Age: Unlimited
* Maximum Supply: 20,000,000

# Suppply

| Blocks | Reward |
| ------ | ------ |
| Block 1 to 100 | Premine 4000000 |
| Block 101 to 400100  | Reward 5 BPC per Block |
| Block 400101 to 844544  | Reward 4.5 BPC per Block |
| Block 844545 to 1344544  | Reward 4 BPC per Block  |
| Block 1344545 to 1915972  | Reward 3.5 BPC per Block |
| Block 1915973 to 2582638  | Reward 3 BPC per Block |
| Block 2582639 to 3382638   | Reward 2.5 BPC per Block |
| Block 3382639 to 4382638  | Reward 2 BPC per Block |
| Block 4382639 to 5715975  | Reward 1.5 BPC per Block |

## Block Explorers

Backpackercoin currently has two explorers.

| Explorer | Link |
| ------ | ------ |
| Primary Explorer | [https://bpcexplorer.com](https://bpcexplorer.com/) |
| Secondary Explore | [https://explorer.bpcexplorer.com](https://explorer.bpcexplorer.com/) |

# Dependencies & Compilation

* Operating System: [Ubuntu 16.04](http://releases.ubuntu.com/16.04/)
* RAM: Minumum 2 GB
* A modern prcoessor with minimum 2 Cores

Install the dependencies in desktop or server:

```sh
$ sudo  apt-get update

# Git
$ sudo  apt-get install git -y

# libssl for cryptography and libevent for Networking
$ sudo  apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils -y

# Boost Utility  for threading, Data Structures etc
$ sudo  apt-get install libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev -y
$ sudo  apt-get install libboost-all-dev -y

# BerkleyDB for wallet support
$ sudo  apt-get install software-properties-common -y
$ sudo  echo | add-apt-repository ppa:bitcoin/bitcoin
$ sudo  apt-get update
$ sudo  apt-get install libdb4.8-dev libdb4.8++-dev -y

# upnp for firewall-jumping support
$ sudo  apt-get install libminiupnpc-dev -y


# QT
$ sudo  apt-get install libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev qttools5-dev-tools libprotobuf-dev protobuf-compiler -y
$ sudo  apt-get install libqt4-dev libprotobuf-dev protobuf-compiler -y

```
Cloning and Compilation:

```sh
# Clone the source code from github
$ https://github.com/backpackercoin577/backpackercoin.git

# Give read write and execute permissions to backpackercoin directory
$ sudo chmod -R 777 backpackercoin

# Compile the source code for cli wallet
$ cd backpackercoin/src && make clean -f makefile.unix && make -f makefile.unix

# Compile the source code for gui wallet
$ cd .. && qmake && make
```

License
====================
Backpackercoin (BPC) Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see http://opensource.org/licenses/MIT.
