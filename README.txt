
http://commotionwireless.net

This is a set of NetworkManager dispatcher scripts for making it easier to
connect to OLSR mesh networks using olsrd.  It is part of the Linux client
for Commotion Wireless  and uses the same profiles as Commotion MeshTether.

https://code.commotionwireless.net/projects/commotion/wiki/Profiles_for_MeshTether

Installing
----------

If you are using Debian, Ubuntu, Mint, or any other Debian-derivative, you can
install Commotion by downloading all .deb packages located at
https://downloads.commotionwireless.net/linux, and installing them with:

sudo dpkg -i \*.deb

If you encounter any dependency errors during this process, simply run:

apt-get install -f

to resolve the problems, and then run the original dpkg command once again.

Bugs
----

If you encounter any problems or wish to request features, please add them to
our issue tracker:

https://github.com/opentechinstitute/nm-dispatcher-olsrd


Building
--------

If you are on a non-Debian-derivitive GNU/Linux distro, then you'll need to
install this manually.  We are looking for contributions of packaging to make
this easy for people to do.

Check the `debian/control` file for a list of standard libraries that are
required.  Here are the other libraries needed:

* https://github.com/opentechinstitute/commotion-linux-py
* https://pypi.python.org/pypi/python-networkmanager

This project relies heavily on the NetworkManager 0.9.x dbus API, currently
via the python-networkmanager library available on pypi:

http://people.redhat.com/dcbw/NetworkManager/NetworkManager%20DBUS%20API.txt
http://projects.gnome.org/NetworkManager/developers/api/09/spec.html
