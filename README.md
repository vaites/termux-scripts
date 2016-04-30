Termux Scripts
==============

A few scripts to automate things with Termux on Android:

* **barcode-scan**: scan a file (or take a photo if not specified) for text or URLs using ZBar package

Installation
------------

Using [Git 2.8.1-2](https://github.com/vaites/termux-packages/commit/11c62dd2484d16cd4cce471166765b8550873956):

    cd && cd ../usr
    mkdir local && cd local
    git clone https://github.com/vaites/termux-scripts.git

Then, just add to your `.profile`:

    export TERMUX_PREFIX=/data/data/com.termux/files/usr
    export PATH=$TERMUX_PREFIX/local/bin:$PATH
