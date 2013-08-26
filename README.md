Setting a Client Group with a pkg
===========

This sample payload-free package will set the Client Group on a computer, before the Monitoring Client's package is installed.

Designed for use with Stéphane Sudre's quite amazing Packages.app

http://s.sudre.free.fr/Software/Packages/about.html


Usage
=====

Download the bits here, and install Packages.

Edit the postinstallation to contain the desired Client Group by placing the desired group name in between the quotes.


    /usr/bin/defaults write /Library/MonitoringClient/ClientSettings ClientGroup -string "Change this Client Group"

Change that client group ;-)


Ensure the script is executable by running a 

    chmod 755 path/to/clientgroup/postinstallation
    
Double Click on com.monitoringclient.clientgroup.pkgproj 

Once Packages is open, choosing Build from the Build menu (or typing Command B) will create the package in the "build" folder.



Contact support@watchmanmonitoring.com with further questions.

