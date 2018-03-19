Build
=====

.. code-block:: bash

  sudo apt-get update
  sudo apt-get install libtalloc-dev uthash-dev libarchive-dev gdb strace realpath
  sudo pip install cpp-coveralls

  make -C src loader.exe loader-m32.exe build.h && env CFLAGS=--coverage LDFLAGS='--coverage' make -C src proot && env PATH=/bin:/usr/bin:/sbin:/usr/sbin:$PWD/src make -C tests



Manuals
=======

- `PRoot <doc/proot/manual.txt>`_

- `CARE <doc/care/manual.txt>`_


Build status
============

- .. image:: https://travis-ci.org/cedric-vincent/PRoot.png?branch=master
     :target: https://travis-ci.org/cedric-vincent/PRoot

- .. image:: https://coveralls.io/repos/cedric-vincent/PRoot/badge.png?branch=master
     :target: https://coveralls.io/r/cedric-vincent/PRoot?branch=master

- .. image:: https://scan.coverity.com/projects/602/badge.svg
     :target: https://scan.coverity.com/projects/602
