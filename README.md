memlog
======

A simple memory visiting log tool based on valgrind

Introduction
------------

This tool follows the instruction of Valgrind Technical Documentation. So it should co-work with Valgrind Core. It is developed with Valgrind 3.8.1.

### Building Instructions

1. Check out the valgrind repository -- `svn co svn://svn.valgrind.org/valgrind/trunk valgrind` or using a release version if you like
2. Go to the valgrind directory -- `cd valgrind` and Check out the memlog repo -- `git clone https://github.com/weichaoguo/memlog.git`
3. Editing -- `Makefile.am`, adding the new directory `memlog` to the TOOLS or EXP_TOOLS variables
4. Editing -- `configure.in`, adding `memlog/Makefile` and `memlog/tests/Makefile` to the `AC_CONFIG_FILES` list
5. Then following the 'GNU automake style' -- `autogen.sh && ./configure --prefix=\`pwd\`/inst && make && make install`

Features
--------

1. Tracing memory address visiting

Links
-----

Valgrind : http://valgrind.org

Contacts
--------

Author: Weichao Guo [guoweichao@mail.com]
