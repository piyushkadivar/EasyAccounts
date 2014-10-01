EasyAccounts is an accounting and inventory control package written in CA-Clipper 5.2. It runs well using DOSBox.

![EasyAccounts screenshot](https://raw.githubusercontent.com/jasim/old-webby-homepage/master/site/content/images/ea_screenshot.png)

You'll need to have a bunch of third party libraries (listed in SRC/EA.LNK) to build it form source. Fortunately they are now available freely from [The Oasis][1]

Feel free to contact me at jasim.ab@gmail.com for any questions or comments regarding this code.

Folder:  SRC
------------
Contains the entire source code of EasyAccounts.

* The main MAKE file is EA.RMK (it is where the information regarding all
 programs and dependencies to be compile is kept)

* The program that starts the application is UTILS.PRG (contains an
INIT PROCEDURE SETVARS which is the first procedure to fire up as the
application is loaded.)

* The main switchboard is the PULLMENU.PRG (contains the entire pulldown
menu and the function names which are called for each task.)

* The E.BAT can be called to compile and link the entire package. But
  you need to have CLIPPER.EXE and BLINKER.EXE in the path, the BIN, LIB and
  INCLUDE path variables should be configured to point to a directory containing the required libraries and header files.


Folder: DOCS
------------
Contains the preliminary documentation of the software.
A word (.doc) file EA_WORD.DOC is present which can be opened in MS-Word.

For viewing other help files, use any text editor, or run the EA-HELP.EXE

Folder: SETUP
-------------
Contains the Binary of the software.
Please run the SETUP.EXE which will create a directory C:\EA and install
the binaries of the software there. The databases are also created
automatically by the setup program.

Please remember the password you give to the SETUP program. It would be
required to log in on the installed EasyAccounts.

The source code of the setup program is SETUP.PRG (SRC folder).
The compile and run batch file is CS.BAT


  [1]: http://www.the-oasis.net/
