FRN-Raspberry-Pi-GPIO
=====================

This is a port of the Client.pm file from Froller. It uses the source from https://code.google.com/p/linux-frn-client/ and
has been modified to use the GPIO pins on the Raspberry-Pi instead of the USB COM-Keyer.

It uses GPIO pin 11 by default but this can be modified in the setPTT.sh file enclosed.

NOTE!
You must start the FRN-Gateway script as root to be able to access GPIO pins on a Raspberry-Pi.

e.g.

cd /opt/LinFRN/bin
sudo FRN-Gateway

If you do not use sudo to start the file as root, then you will get an error message which is quite cryptic and will look something like this:

Enter new
About to run
bcm2835_init: Unable to open /dev/mem: Keine Berechtigung
Could not init BCM2835 library at /home/pi/perl5/lib/perl5/Net/FRN/Client.pm line 214, <FH> line 46.
aplay: playback:2483: Lesefehler

YOU HAVE BEEN WARNED!
