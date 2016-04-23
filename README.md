Setting a Client Group with a pkg
===========

Or, running any other script via the `Resources/postinstallation`

This sample payload-free package will set the Group on a computer, ideal for use before deploying your Monitoring Client package.

Designed for use with Stéphane Sudre's quite amazing [Packages.app](http://s.sudre.free.fr/Software/Packages/about.html)


Usage
=====

- Install Packages, if it isn't already

- Fork or Check out this repository

- Edit the postinstallation to contain the desired Group by placing the desired group name in between the quotes.


    `/usr/bin/defaults write /Library/MonitoringClient/ClientSettings ClientGroup -string "ENTER_GROUP_NAME"`


- Add any other tasks you need run, each on their own line (following normal bash syntax)

Double Click on ![Packages icon](Resources/packages.png)`com.monitoringclient.clientgroup.pkgproj` 



Once Packages is open, choosing Build from the Build menu (or typing Command B) will create the package in the "Build" folder.



Questions? Open an issue or email support@watchmanmonitoring.com

