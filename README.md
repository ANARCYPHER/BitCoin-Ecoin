E-coin integration/staging tree 
================================
COIN CREATED FOR FUN
================================

https://www.e-coin.com

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Litecoin Developers
Copyright (c) 2019 E-coin Developers
What is E-coin?
----------------
Cryptographic currency created in my spare time, in reference to the TV series Mr. Roboot, for which a corporation called ECORP. created a currency a (ECOIN). Being a huge fan of the series, I decided to create this coin just for fun
Ecoin is similar to Bitcoin, some differences are listed here.

 - subsidy halves in 940k blocks (~4 years)
 - ~94 million total coins
 - 50 coins per block
 - 288 blocks to retarget difficulty
 
 we created this cryptocurrency in my spare time, and for liking the Mr.robot TV series

Ecoin is a litecoin fork and almost everything is the same as litecoin, with some modifications made to further streamline transactions.

For more information, as well as an immediately useable, binary version of
the Ecoin client sofware, see https://www.e-coin.com.

License
-------

Ecoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Ecoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/ecoin-project/ecoin/tags) are created
regularly to indicate new official, stable release versions of Ecoin.

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
    ./ecoin-qt_test

