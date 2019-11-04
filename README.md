![GitHub Logo](/src/qt/res/images/splash.png)

Twitcoin integration/staging tree
================================

http://www.twit.rocks

Copyright (c) 2009-2014 Bitcoin Developers <br>
Copyright (c) 2011-2014 Litecoin Developers <br>
Copyright (c) 2018 Twitcoin Developers

What is Twitcoin?
----------------
![GitHub Logo](/src/qt/res/icons/bitcoin.png) <br>
Coin Name: Twitcoin <br>
Ticker: TWIT <br>
Algorithm: Script <br>
Type: PoW

Maximum Coin Supply: 330.000.000 <br>
Premine: 33.000.000 <br>
Useage: Team, Airdrops, Bounties (Marketing, Design, Etc.)

Block time: 30 seconds <br>
Maturity: 30 Blocks <br>
Difficulty Re-adjustment: 330 Blocks

Block rewards: <br>
Phase 1 - Premine (Block 1) 33.000.000 TWIT <br>
Phase 2 - PoW (Block 2-1337) .50 TWIT <br>
Phase 3 - PoW (Block 1338+) 30 TWIT

For more information, as well as an immediately useable, binary version of
the Twitcoin client sofware, see http://www.twit.rocks.

License
-------

Twitcoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Twitcoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/twitrocks/twitcoin/tags) are created
regularly to indicate new official, stable release versions of Twitcoin.

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
    ./twitcoin-qt_test

