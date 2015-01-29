# BankID autolaunch test for Chrome on Android

This simply tests what happens when window.location is set to an intent URL opening the BankID app.

The problem is that Chrome will load the previous page in the background so when the user goes back / is done in the BankID app she/he lands not on the "originating" page but the previous.

An user originated window.location rewrite does not suffer from this.

## Running

Simply fire up a web server and go, say:

    > python -m SimpleHTTPServer

