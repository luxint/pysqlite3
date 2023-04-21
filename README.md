pysqlite3 with encryption
=========================

This library takes the SQLite module from Python 3 and packages it as a
separately-installable module.

Intended to be used with the amalgamation files from https://github.com/utelle/SQLite3MultipleCiphers
to build an encryption enabled SQLite to be used in python.


Building a statically-linked library
------------------------------------
Download the amalgamation files from https://github.com/utelle/SQLite3MultipleCiphers/releases
```
# Copy the sqlite3mc_amalgamation files into the root of the pysqlite3 checkout
# and run build_static + build:
$ cp sqlite/sqlite3.[ch] pysqlite3/
$ cd pysqlite3
$ python setup.py build_static build
```

You now have a statically-linked, encryption enabled completely self-contained `pysqlite3`.
