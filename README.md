# getinfected

**Repo:** OATSEA/getinfected
**Version:** 0.2
**Author:** Harry Longworth
**Contributors:** Vishal Simon, Harry Longworth & OATSEA Team
**Website:** teachervirus.org

##About
**getinfected** is the initial teacher virus PHP infection script that is used to install the core teachervirus files.  

It consists of a single file **getinfected.php** in order to simplify deployment for users. 

This file fetches the core Teacher Virus files.  It also enables updates and device to device installation.

**NOTE: ** Teacher Virus is only viral from a philosophical perspective - it can not infect a device without the consent of the administrator/owner of the device (installation action required).

##For Android:
The getinfected.php file is fetched by the android app (teachervirus.apk).

##For Other Devices
Teacher Virus operates on any devices with a compatible webserver (HTML/PHP/SQLite) and sufficient rights.

For installation on these devices the getinfected.php file needs to be placed in the root of the webserver's public folder (i.e. htdocs) and opened. 

##Assumptions
To keep things simple we make the following assumptions at this point:
* getinfected.php will be in the root folder of the webserver.

##What's New? 
With version 0.2 we introduce the following improvements:
* ability to select which branch to install from github
* ability to remove the previous installation
* ability to selectively delete components of the previous installation - for example you now have the ability to not delete the data folder so that the administrator password is kept or not delete payload folders so that payloads don't have to be downloaded again.
* ability to reinstall using the version of Teacher Virus previously downloaded so that you don't have to re-download it again when you're just doing a reinstall to get back to a clean build.
* better error handling.
* alternative download mechanisims (CURL and Copy) to handle device compatibility issues.
* ability to control debug text so that you can show or not show detailed installation comments.
* ability to install from an infected device based on url or IP address and to set the port required by that device (e.g. 8080 for androids or no port for standard webservers working on port 80)
* access to getinfected.php is now controlled by pattern lock security if Teacher Virus is already installed (based on use of 0.2 version of Teacher Virus)
* back button to return to the admin interface if Teacher Virus is already installed

##Wishlist Issues
We are always looking for suggestions and feedback on each release so that we can prioritise functionality required for the next sprint.  At the moment we are looking at working on the following capabilities for the next phase of development:

* simplification of Android deployment by integration of the webserver component with the Android webapp with the goal of publishing the platform to Google Play to simplify deployment.
* ability to update getinfected.php and determine the need to do so.
* ability to check for availability of "updates" to Teacher Virus based on version.
* ability to install based on release version rather than just branch (default is master branch)
* multi-lingual interface (and a Swahili version of the interface in order to meet the requirements of the Global Learning XPRIZE)

##Known Issues:
* There known deployment issues with Android version 5 that we are investigating
* Further investigation required into security aspects of use on public webservers



