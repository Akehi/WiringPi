This is modified version !!
===========================

This is modified version of "Unofficial WiringPi Mirror" for RPi4 + Ubuntu Server 18.04.
It seems to work for me but I can't ensure safe operation.
I just conbined and did below operations without understanding WiringPi program.
Good luck for ROS/ROS2 user.

1. Apply eaon patch to WiringPi 2.50
WiringPi2.50 for ubuntu19 package is available.
Patch files are supplied here.
 wget http://archive.ubuntu.com/ubuntu/pool/universe/w/wiringpi/wiringpi_2.50-0ubuntu1.debian.tar.xz
with applying this patch to original source, WiringPi works on ubuntu18 + RPi1-3

2. Merge Wiring2.60 and 2.50-patched
WiringPi2.50 is not available on RPi4 because BCMxxx is deferent from other RPi.
WiringPi2.60 is available on RPi4.
with merging Wiring2.60 and 2.50-patched , WiringPi works on ubuntu18 + RPi4

Note
====

This is an unofficial mirror of WiringPi to support ports (Python/Ruby/etc).

Please do not email Gordon if you have issues, he will not be able to help.

Pull-requests are not currently accepted, since this is a mirror.

For support, comments, questions, etc please join the WiringPi Discord channel: https://discord.gg/SM4WUVG

wiringPi README
===============

Please note that the official way to get wiringPi is via git from
git.drogon.net and not GitHub.

ie.

  git clone git://git.drogon.net/wiringPi

The version of wiringPi held on GitHub by "Gadgetoid" is used to build the
wiringPython, Ruby, Perl, etc. wrappers for these other languages. This
version may lag the official Drogon release.  Pull requests may not be
accepted to Github....

Please see

  http://wiringpi.com/

for the official documentation, etc. and the best way to submit bug reports, etc.
is by sending an email to projects@drogon.net

Thanks!

  -Gordon
