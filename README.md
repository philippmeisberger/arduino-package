Arduino Package
===============

[![Build Status](https://travis-ci.org/philippmeisberger/arduino-package.svg?branch=master)](https://travis-ci.org/philippmeisberger/ardunio-package)

Utility to build Debian package from Arduino binary distribution.

Building
--------

Install required packages

    ~# apt-get install git devscripts

Clone this repository

    ~$ git clone https://github.com/philippmeisberger/arduino-package.git

Build the package

    ~$ cd ./arduino-package/
    ~$ dpkg-buildpackage -uc -us

Install the package

    ~# dpkg -i ../arduino-package*.deb

Usage
-----

Download Arduino .tar.xz archive file from <https://www.arduino.cc> and execute `make-arduinopkg` with the downloaded file as argument. The Debian package is built in the current directory.

Installation of Arduino IDE
---------------------------

Install package

    ~# dpkg -i arduino*.deb

Finally install missing dependencies

    ~# apt-get install -f

Questions and suggestions
-------------------------

If you have any questions to this project just ask me via email:

<team@pm-codeworks.de>
