See readme-qt.rst for instructions on building Rubycoin QT, the graphical user interface.

PPC is not supported because it's big-endian.


# Instructions

* Install XCode with all the options checked. The current version is available from http://developer.apple.com

* Clone from Github to get the source code:

`git clone https://github.com/rubycoinorg/rubycoin.git rubycoin`

* Download and install MacPorts from http://www.macports.org/

* Install dependencies from MacPorts

`sudo port install boost db48 openssl miniupnpc`

* Optionally install qrencode (and set USE_QRCODE=1)

`sudo port install qrencode`

* Now you should be able to build rubycoind:

`cd rubycoin/src`

`make -f makefile.osx`

Run:
  `./rubycoind --help`  # for a list of command-line options.
  
Run
  `./rubycoind -daemon` # to start the rubycoin daemon.
  
Run
  `./rubycoind help` # When the daemon is running, to get a list of RPC commands
