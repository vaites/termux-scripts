Termux Scripts
==============

A few scripts to automate things with Termux on Android:

* **barcode-scan**: scan a file (or take a photo if not specified) for text or URLs using ZBar package
* **ocr-scan**: scan a file (or take a photo if not specified) for text Tesseract package
* **php-web-server**: start the built-in PHP web server displaying the IP address to connect to

Installation
------------

Using at least [Git 2.8.1-2](https://github.com/vaites/termux-packages/commit/11c62dd2484d16cd4cce471166765b8550873956):

    cd && cd ../usr
    mkdir local && cd local
    git clone https://github.com/vaites/termux-scripts.git

Then, just add to your `.profile`:

    export TERMUX_PREFIX=/data/data/com.termux/files/usr
    export PATH=$TERMUX_PREFIX/local/bin:$PATH
