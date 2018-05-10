* **Testing only! Will not work on main net with test settings**

* **Install from source**

  This involves downloading the source, meeting the dependencies, compiling the code, and then installing the resulting software. 

   git clone https://github.com/cygnusxi/CurecoinSource.git

    FOR THE GUI CLIENT:

    > 1. **sudo apt-get install qt5-default qt5-qmake qtbase5-dev-tools qttools5-dev-tools libboost-dev libboost-system-dev libboost-filesystem-dev libboost-program-options-dev libboost-thread-dev libssl-dev libminiupnpc-dev libdb5.3++-dev dh-make build-essential** .  sudo apt-get install libssl1.0-dev <-- Might be needed if build fails 
    > 2. From the main directory, run the following:
    > 3. **qmake && make**

    FOR THE HEADLESS CURECOIND:

    > 1. **sudo apt-get install libboost-all-dev libqrencode-dev libssl-dev libdb5.3-dev libdb5.3++-dev libminiupnpc-dev dh-make build-essential**
    > 2. **cd src**
    > 3. **make -f makefile.unix**
    > 4. **sudo make install** Alternatively, don't run that command and just place the binary wherever you want.

    libdb4.8 should also work if libdb5.1 is too high a version for you. Newer versions of Linux will need libdb5.3++-dev

