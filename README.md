PlanetDollar (PDR)
================================

http://www.planetdollar.org

Copyright (c) 2009-2013 Bitcoin Developers

Copyright (c) 2013-2014 Ronpaulcoin Developers 

Copyright (c) 2014 RealStackCoin Developers

Copyright (c) 2014 PlanetDollar Developers

Proof-of-work algorithm:
 - Scrypt n Factor
 - Premine: 1 200 000 000 000 (1.2 trillion..matching USD circulation)
 - Mining Reward size: 100 per block to start +5 each day, until 60k rewards.
 - Resulting Inflation: starts at 0.1% -> ~1%, then starts decreasing again
    - rewards stop at block: 19215338410114
 - 2.5 minute block targets 
 - Confirmations? 6
 - Transaction cost min: 0.01  
 - KGW implementation

default Port 7784  / +10k for test net
default RPC port 7783 

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./Realstackcoin-qt_test

