
http://commotionwireless.net

This is a set of NetworkManager dispatcher scripts for making it easier to
connect to OLSR mesh networks using olsrd.  It is part of the Commotion
project and uses the same profiles as Commotion MeshTether.

https://code.commotionwireless.net/projects/commotion/wiki/Profiles_for_MeshTether

How to setup on Debian/Ubuntu/etc.

 sudo add-apt-repository ppa:guardianproject/commotion
 sudo apt-get install python-networkmanager python-pyjavaproperties psmisc olsrd olsrd-plugins


This project relies heavily on the NetworkManager 0.9.x dbus API, currently
via the python-networkmanager library available on pypi:

http://people.redhat.com/dcbw/NetworkManager/NetworkManager%20DBUS%20API.txt
http://projects.gnome.org/NetworkManager/developers/api/09/spec.html
