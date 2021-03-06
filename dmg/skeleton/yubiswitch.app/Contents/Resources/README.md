yubiswitch
==========

Author: Angelo "pallotron" Failla <pallotron@freaknet.org>

`yubiswitch` is an OSX status bar application to enable/disable a Yubikey.

This is particularly useful if you use to keep the yubikey plugged into your
USB slots while carrying your laptop around. It avoids your vim sessions, or
your terminal sessions to be filled with `ejehlrlrclcllukjgehhrttbknnbjdfn` :D

Known Issues
============

* This app only works with a single model of yubikey, the *YubiKey Nano*.
That is the small model that fits cleanly into your usb port (idVendor 0x1050
and idProduct 0x0010) and you can enable by touching the golden stripe with
your finger tip.

* This app only works with recent version of OSX because it relies on the
Notification Centre. 10.8.x and above would do it.

TODO and future plans
=====================

* Feature: lock computer when yubikey is removed
* Make hotkey configurable via configuration window, currently it's static and
it is cmd-Y
* Support more yubikeys nano on multiple USB slots

Credits
=======

Credits to Anton Tolchanov (@knyar), he originally wrote this in Python using
PyObjC bridge. I decided to port this into Objective-C when I found out that
Carbon Event Manager libs have been removed from Python3.
See http://docs.python.org/2/library/carbon.html
