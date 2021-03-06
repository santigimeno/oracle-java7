Please note that Java 7 reached its end of public updates and Oracle
will not release any more updates after April 2015. For details
please see http://www.oracle.com/technetwork/java/eol-135779.html

Introduction
------------

Java 7 packages for Debian.

Supported Debian versions
-------------------------

So far packages were tested on following Debian versions:

- jessie i386/amd64
- wheezy i386/amd64
- squeeze i386/amd64

New users of Debian Wheezy should cosider using java-package:
<http://wiki.debian.org/JavaPackage>

I do not have resources to test packages on Ubuntu. However, if one
finds any problem on Ubuntu, feel free to report an issue and I will
try to resolve it.

Usage
-----

To create packages on your own:

- apt-get install debhelper curl unzip
- git clone git://github.com/rraptorr/oracle-java7.git
- cd oracle-java7
- sh ./prepare.sh
- dpkg-buildpackage -uc -us
- install any missing packages that dpkg-buildpackage complains about
  and repeat

Legal
-----

Oracle does not permit to distribute repackaged binaries of Java, so
be advised that hosting any public repository with Java packages is
probably illegal (at least in some parts of the world).

On the other hand, this repository contains only scripts, that allows
one to repackage Oracle Java in Debian friendly way. No binaries are
or will be hosted.

Thanks
------

If this saved you some time you can thank me with some bitcoins:
1java7mij3BHAw8eWqjr1qFGrDipyq5LN
