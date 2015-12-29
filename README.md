# getinfected

**Repo:** OATSEA/getinfected
**Version:** 0.5 [DEV]
**Date:** Nov 2015
**Author:** Harry Longworth
**Contributors:** Vishal Simon, Harry Longworth & OATSEA Team
**Website:** teachervirus.org

##About
**getinfected** is the initial teacher virus PHP infection script that is used to install the core teachervirus files.  

It consists of a single file **getinfected.php** in order to simplify deployment for users. 

This file fetches the core Teacher Virus files.  It also enables updates and device to device installation.

**NOTE: ** Teacher Virus is only viral from a philosophical perspective - it can not infect a device without the consent of the administrator/owner of the device (installation action required).

##For Android:
The getinfected.php file is included in the android app (teachervirus.apk).

##For Other Devices
Teacher Virus operates on any devices with a compatible webserver (HTML/PHP/SQLite) and where you have sufficient rights.

For installation on these devices the getinfected.php file needs to be placed in the root of the webserver's public folder (i.e. htdocs) and opened in a browser. 

##Assumptions
To keep things simple we make the following assumptions at this point:
* getinfected.php will be in the root folder of the webserver (although efforts have been made to support subfolder installs).

##What's New? 
With version 0.5 we introduce the following improvements:
* to be determined
* 
##Wishlist Issues
We are always looking for suggestions and feedback on each release so that we can prioritise functionality required for the next sprint.  At the moment we are looking at working on the following capabilities for the next phase of development:

* to be determined

##Known Issues:
* There known deployment issues with Android version 5 that we may not be able to resolve
* Further investigation required into security aspects of use on public webservers



