pysqlite3
=========

This library takes the SQLite module from Python 3 and packages it as a
separately-installable module.

Intended to be used with the amalgamation files from https://github.com/utelle/SQLite3MultipleCiphers
to build a encryption enabled SQLite to be used in python.


Building a statically-linked library
------------------------------------

```
# Copy the sqlite3mc_amalgamation files into the root of the pysqlite3 checkout
# and run build_static + build:
$ cp sqlite/sqlite3.[ch] pysqlite3/
$ cd pysqlite3
$ python setup.py build_static build
```

You now have a statically-linked, encrytion enabled completely self-contained `pysqlite3`.
