

Cryptcoin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 1 minute block targets
 - subsidy halves in 10k blocks.
 - 25 coins per block
 - 1 day to retarget difficulty
 - 25 blocks coinbase muturity





### Testing

cd src; make -f makefile.unix ;

./cryptocoind -deamon


# Create a cryptocoin.conf file inside /home/username/.cryptocoin/

rpcuser=Yourusername
rpcpassword=Yourpassword
addnode=192.168.0.1



Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./cryptcoin-qt_test
