
#shapelib

Shapefile C Library (origin at http://shapelib.maptools.org)

---

Building on Unix
----------------

1) Edit Makefile, and set CFLAGS, and CC macros as required for the
   target system.  Often the defaults will work fine.

2) type "make" 

The result should be:

Core shapelib support.  
  shpopen.o
  dbfopen.o
  safileio.o
  shptree.o
  libshp.a

Utility/demonstration programs:
  shpcreate, shpdump, shpadd, dbfcreate, dbfdump, dbfadd, shptreedump

3) To test type:
  make test

4) To libshp.a and the test binaries in /usr/local:
  make install 

---

Building on Windows
-------------------

If you have run the VC++ VCVARS32.BAT, you should be able to type the 
following in a command window to build the code and executables:

C:>  nmake /f makefile.vc 

Otherwise create your own VC++ project.  There aren't many files to deal with
here!

