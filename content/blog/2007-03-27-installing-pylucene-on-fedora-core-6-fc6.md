---
author: admin
date: 2007-03-27 23:14:37+00:00
draft: false
title: Installing PyLucene on Fedora Core 6 (FC6)
type: post
url: /2007/03/28/installing-pylucene-on-fedora-core-6-fc6/
categories:
- Technical
tags:
- fedora
- fedora-core-6
- gcj
- lucene
- pylucene
- Python
---

This is just one of those "I wish someone else had written this before I tried to do it" posts. Unlike most popular software on Fedora or indeed in Python, there is no simple installer for PyLucene and no binary that you can use yum or rpm to install with. The install instructions have a whiff of something from around 1997 rather than 2007. Almost a case of "if you can't figure out how to install it, you don't deserve to use our software".

So for other poor schmucks who find themselves stuck around midnight trying to install PyLucene on a reasonably updated FC6 (as of March 27th 2007), all you need to do is:

Grab the latest source from http://downloads.osafoundation.org/PyLucene/src/
I used http://downloads.osafoundation.org/PyLucene/src/PyLucene-src-2.1.0-2.tar.gz

Unzip, cd to the source dir and edit the Makefile

At the top of the Makefile, make sure to comment out any mentions of Berkeley DB as follows:

`
VERSION=2.1.0-2
LUCENE_SVN_VER=509013
LUCENE_VER=2.1.0-$(LUCENE_SVN_VER)
LUCENE_SVN=http://svn.apache.org/repos/asf/lucene/java/trunk
PYTHON_VER=2.4
#DB_VER=4.3.29
#DB_VER=4.4.20
#DB_VER=4.5.20

PYLUCENE:=$(shell pwd)
LUCENE=lucene-java-$(LUCENE_VER)
#DB_LIB_VER=$(basename $(DB_VER))
`

Then scroll down to the bit for Linux and set it up like this (defaults were wrong for Fedora):

`
# Linux
PREFIX=/usr/local
PREFIX_PYTHON=/usr
LIBDIR_NAME=lib
GCJ_HOME=/usr
GCJ_LIBDIR=$(GCJ_HOME)/$(LIBDIR_NAME)
GCJ_STATIC=0
LIB_INSTALL=libstdc++.so.6 libgcc_s.so.1
#DB=$(PYLUCENE)/db-$(DB_VER)
#PREFIX_DB=$(PREFIX)/BerkeleyDB.$(DB_LIB_VER)
ANT=ant
PYTHON=$(PREFIX_PYTHON)/bin/python
`

Save and exit

You now need to make one link to a gcc library as follows:

`
ln -s  /usr/lib/gcc/i386-redhat-linux/4.1.1/libgcc_s.so /usr/lib/libgcc_s.so.1
`

Note that the 4.1.1 part may change if you have a slightly older/newer FC6

Then all you need to do is
`
make
make install
`

Hurrah. Soda pop and pretzels for all.
