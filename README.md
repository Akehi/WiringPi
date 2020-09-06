This is modified version !!
===========================

This is modified version of "Unofficial WiringPi Mirror" for RPi4 + Ubuntu Server 18.04.
Clone the branch "for_rpi_ubuntu18" and sudo ./build.
Then it works for me but I can't ensure safe operation.
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


Unofficial WiringPi Mirror
==========================

This is an unofficial mirror of WiringPi to support ports (Python/Ruby/etc).  With the
[end of official development](http://wiringpi.com/wiringpi-deprecated/), this repository
has become a mirror of the last "official" source release as well as a source for small
updates to support newer hardware (primarily for use by the ports).

  * The final "official" source release can be found at the
    [`final_source_2.50`](https://github.com/WiringPi/WiringPi/tree/final_official_2.50) tag.
  * The default `master` branch contains code that has been written since that final source
    release to provide support for newer hardware.

Please do not email Gordon if you have issues, he will not be able to help.

Pull-requests may be accepted to add or fix support for newer hardware, but new features or
other changes will not be accepted.

For support, comments, questions, etc please join the WiringPi Discord channel: https://discord.gg/SM4WUVG
