
# OpCon Web Installer

The OpCon Web Installer (OWI) is a tool designed to make the process of installing and maintaining OpCon software easier.  It has the ability to connect to the [public distribution location of OpCon software](https://files.smatechnologies.com) automatically and download or install selected product components.

## Installation

To use the OWI tool, simply browse to the [latest release](https://github.com/smatechnologies/opcon-web-installer/releases/latest) of this repository and download the assets.  It should be a single zip file named OpConWebInstaller.zip.  Unzip this archive file, and you are ready to begin!  Double-click the application executable to launch the program.

> ***Note:*** The application does not handle your license file.  Please follow standard procedures for acquiring and applying it.

As new versions are made available, as long as the machine from which the application is running has access to this repository, it will detect and ask users to update to the latest version.  If a machine does not have access, users should follow the same steps they did on initial installation and simply download the latest release's assets.

For information specific to an OpCon product component's installation, please see the [OpCon installation guide](https://help.smatechnologies.com/opcon/core/latest/index.htm#Files/Installation/Overview.htm).

## Feedback

Please provide feedback through standard channels.

Enhancement ideas should be submitted via the [SMArt ideas portal](https://smartideas.ideas.aha.io/portal_session/new) with the component of **OpCon Web Installer** selected.

To report an issue, please use the [Customer Community](https://smatechnologies.force.com/smartusers/login]) and open a Support case.  We will ask you to be on the latest version.  If you are encountering issues please check here to verify you have the latest!

## Release Notes

### 1.0.1 - November 30, 2020
#### Improvements & Fixes
- Added the following items with Windows installers:
    - **SMA OpCon** (the 20.00 consolidated replacement for *SMA OpCon Database Scripts*, *SMA OpCon SAM*, *SMA OpCon Solution Manager*)
    - **SMA OpCon Documentation** (available for 19.1 and previous releases only, please use [https://help.smatechnologies.com](https://help.smatechnologies.com) for current documentation)
- Removed the following items with Windows installers:
    - **SMA OpCon Enterprise Manager x64 (No Reports)**
    - **SMA OpCon Enterprise Manager x86 (No Reports)**
    - **SMA OpCon Enterprise Manager x86**

### 1.0.0 - September 28, 2020
#### New Features 
- Runs available Windows installers in the required order for successful installation or upgrade. 
- Grants the ability to download or install (which will also download as a pre-requisite) installers from the distribution location.
- Has the ability to run the installers from a filesystem rather than looking for the latest on the internet.
- Has the ability to uninstall product components.
- Works across OpCon component versions.  The same OpCon Web Installer can be used to upgrade from 19.0.x to 20.0.x and can also install a different or new version of an agent or connector.
- Has the ability to self-update itself (not the OpCon components) and will notify users when updates are available. 

