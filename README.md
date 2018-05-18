Vologold integration/staging tree
================================

http://www.vologold.com

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 LiteCoin Developers
Copyright (c) 2014-2018 VoloGold Developers
What is Vologold?
----------------

Vologold is a 15 years blockchain based cryptocurrency using scrypt as a proof-of-work algorithm.
 - 3 minute block targets
 - subsidy halves in 740k blocks (~1 years)
 - 6.9 millions total coins

Main specs of the VoloGolg (VLG) cryptocurrency.
 - 10 coins per block
 - 240 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Vologold client sofware, see http://www.vologold.com
License
-------

Vologold is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Vologold
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/vologold-project/vologold/tags) are created
regularly to indicate new official, stable release versions of Vologold.

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

    qmake VOLOGOLD_QT_TEST=1 -o Makefile.test vologold-qt.pro
    make -f Makefile.test
    ./vologold-qt_test

# vologold
