gopro-wifi-API
==============

An Java-API to control a Gopro remotely via http requests.
It's a copy of the http://goprojavaapi.blogspot.com/ https://code.google.com/p/goprojavaapi/source/checkout I tried to contact the person behind it, but never got an answer.
How to install (http://goprojavaapi.blogspot.com.br/2013/10/how-download-gopro-java-code.html)

On some parts it seems unfinished I fixed it here and there and that's why I'm putting it on GitHub, because it's a slightly improved version.
But honstely I didn't have the time to go through all the possible requests and test them.


(copy past from the GoPro URL.txt)
The general query structure is  : http://<ip>/<device>/<app>?t=<password>&p=<command>
 
Where:<device> can be bacpac or camera.
 
From the page, we can extract the following queries;
 
Turn on camera : http://<ip>/bacpac/PW?t=<password>&p=%01
Turn off camera : http://<ip>/bacpac/PW?t=<password>&p=%00
Change mode    : http://<ip>/bacpac/PW?t=<password>&p=%02
 
Start capture : http://<ip>/bacpac/SH?t=<password>&p=%01
Stop capture : http://<ip>/bacpac/SH?t=<password>&p=%00
 
Preview
On : http://<ip>/camera/PV?t=<password>&p=%02
Off : http://<ip>/camera/PV?t=<password>&p=%00
 
Mode
Camera     : http://<ip>/camera/CM?t=<password>&p=%00
Photo        : http://<ip>/camera/CM?t=<password>&p=%01
Burst         : http://<ip>/camera/CM?t=<password>&p=%02
Timelapse : http://<ip>/camera/CM?t=<password>&p=%03
Timelapse : http://<ip>/camera/CM?t=<password>&p=%04
 
Orientation
Head up     : http://<ip>/camera/UP?t=<password>&p=%00
Head down : http://<ip>/camera/UP?t=<password>&p=%01
 
Video Resolution
WVGA-60  : http://<ip>/camera/VR?t=<password>&p=%00
WVGA-120  : http://<ip>/camera/VR?t=<password>&p=%01
720-30   : http://<ip>/camera/VR?t=<password>&p=%02
720-60   : http://<ip>/camera/VR?t=<password>&p=%03
960-30   : http://<ip>/camera/VR?t=<password>&p=%04
960-60   : http://<ip>/camera/VR?t=<password>&p=%05
1080-30 : http://<ip>/camera/VR?t=<password>&p=%06
 
FOV
wide : http://<ip>/camera/FV?t=<password>&p=%00
medium : http://<ip>/camera/FV?t=<password>&p=%01
narrow : http://<ip>/camera/FV?t=<password>&p=%02
 
Photo Resolution
11mp wide     : http://<ip>/camera/PR?t=<password>&p=%00
8mp medium  : http://<ip>/camera/PR?t=<password>&p=%01
5mp wide       : http://<ip>/camera/PR?t=<password>&p=%02
5mp medium  : http://<ip>/camera/PR?t=<password>&p=%03
 
Timer
0,5sec : http://<ip>/camera/TI?t=<password>&p=%00
1sec    : http://<ip>/camera/TI?t=<password>&p=%01
2sec    : http://<ip>/camera/TI?t=<password>&p=%02
5sec    : http://<ip>/camera/TI?t=<password>&p=%03
10sec  : http://<ip>/camera/TI?t=<password>&p=%04
30sec  : http://<ip>/camera/TI?t=<password>&p=%05
60sec  : http://<ip>/camera/TI?t=<password>&p=%06
 
Localisation
On : http://<ip>/camera/LL?t=<password>&p=%01
Off : http://<ip>/camera/LL?t=<password>&p=%00
 
Bip Volume
0%     : http://<ip>/camera/BS?t=<password>&p=%00
70%   : http://<ip>/camera/BS?t=<password>&p=%01
100% : http://<ip>/camera/BS?t=<password>&p=%02
 
Edited : added more commands
