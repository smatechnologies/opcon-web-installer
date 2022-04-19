# OpCon Web Installer

The OpCon Web Installer (OWI) is a tool designed to make the process of installing and maintaining OpCon software easier.  It has the ability to connect to the [public distribution location of OpCon software](https://files.smatechnologies.com) automatically and download or install selected product components.

## Installation

To use the OWI tool, simply browse to the [latest release](https://github.com/smatechnologies/opcon-web-installer/releases/latest) of this repository and download the assets.  It should be a single zip file named OpConWebInstaller.zip.  Unzip this archive file, and you are ready to begin!  Double-click the application executable to launch the program.

> ***Note:*** For web downloads, the machine will require access to **files.smatechnologies.com** on ports **443** and **990**.

> ***Note:*** The application does not handle your license file.  Please follow standard procedures for acquiring and applying it.

As new versions are made available, as long as the machine from which the application is running has access to this repository, it will detect and ask users to update to the latest version.  If a machine does not have access, users should follow the same steps they did on initial installation and simply download the latest release's assets.

> ***Note:*** For self-updating, the machine will require access to **github.com** on port **443**.

For information specific to an OpCon product component's installation, please see the [OpCon installation guide](https://help.smatechnologies.com/opcon/core/latest/index.htm#Files/Installation/Overview.htm).

## Feedback

Please provide feedback through standard channels.

Enhancement ideas should be submitted via the [SMArt Ideas Portal](https://smartideas.featureupvote.com) with the component of **OpCon Web Installer** selected.

To report an issue, please use the [Customer Community](https://smatechnologies.force.com/smartusers/login) and open a Support case.  We will ask you to be on the latest version.  If you are encountering issues please check here to verify you have the latest!

## Release Notes

### 1.7.0
##### March 14, 2022
#### Improvements & Fixes
- Fixed issue where Connectors that have been converted to ZIP packages for install were not showing the correct available operations.

### 1.6.0
##### December 17, 2021
#### New Features
- New SAFE MODE option on the welcome page removes all actions except DOWNLOAD from the package list.

### 1.5.0
##### November 22, 2021
#### New Features
- New wizard that displays when previous packages are found installed and offers to update all to the latest version.

#### Improvements & Fixes
- Remove settings page and move to settings bar above packages list.  Filters are now applied in real-time.

### 1.4.0
##### October 12, 2021
#### New Features
- Customers are now able to leverage the Online Web Installer (OWI) to manage the installation and update process for supported connectors.

### 1.3.0
##### September 22, 2021
#### New Features
- Customers will now have the ability to access and download the OpCon Web Installer (OWI) from a publicly hosted SMA FTP location.

#### Improvements & Fixes
- Fixed an issue where installation would still be attempted even when downloading the installer failed.
- Improved speed and reliability for file transfers.

### 1.2.0
##### March 01, 2021
#### New Features
- OpCon Deploy's ImpEx2 server component now has its own installer and will be available with the OpCon package with the same release cadence. This makes it easy to upgrade ImpEx2 only when needed without having to upgrade OpCon or Deploy client. It also makes it easy to upgrade Deploy client without upgrading ImpEx2 or OpCon.

#### Improvements & Fixes
- Modified priority list to ensure Configuration Utility is installed/updated before SMA OpCon

### 1.1.0
##### January 11, 2021
#### New Features
- Added the ability to download non-Windows based agents from the internet.
- Added a new setting, **Show Short-Term Support (STS) Releases**, that controls whether or not STS releases are displayed to users.  The default value is false.
- Added a new setting, **Show All Components**, that controls whether product components that are no longer part of the latest release are displayed.  The default value is false.

#### Improvements & Fixes
- Application configuration settings now have tooltips that provide more information about each option.  The *Location* step is now named *Settings*.
- Application configuration is now saved to a *config.yml* file in the application directory.
- Updated the setting selection for searching locally or the internet for packages to a checkbox named **Offline Mode**.  The default is false.
- Fixed an issue where Microsoft-based agents would incorrectly show as not installed when they were present on the system.
- Fixed the installer priority to always run SMA OpCon before installing other non-deprecated installers.
- Simplified the requirements for web downloads.  Machines now require access to files.smatechnologies.com on ports 443 and 990 for the ability to download new versions from the internet.

### 1.0.1
##### November 30, 2020
#### Improvements & Fixes
- Added the following items with Windows installers:
    - **SMA OpCon** (the 20.00 consolidated replacement for *SMA OpCon Database Scripts*, *SMA OpCon SAM*, *SMA OpCon Solution Manager*)
    - **SMA OpCon Documentation** (available for 19.1 and previous releases only, please use [https://help.smatechnologies.com](https://help.smatechnologies.com) for current documentation)
- Removed the following items with Windows installers:
    - **SMA OpCon Enterprise Manager x64 (No Reports)**
    - **SMA OpCon Enterprise Manager x86 (No Reports)**
    - **SMA OpCon Enterprise Manager x86**

### 1.0.0
##### September 28, 2020
#### New Features 
- Runs available Windows installers in the required order for successful installation or upgrade. 
- Grants the ability to download or install (which will also download as a pre-requisite) installers from the distribution location.
- Has the ability to run the installers from a filesystem rather than looking for the latest on the internet.
- Has the ability to uninstall product components.
- Works across OpCon component versions.  The same OpCon Web Installer can be used to upgrade from 19.0.x to 20.0.x and can also install a different or new version of an agent or connector.
- Has the ability to self-update itself (not the OpCon components) and will notify users when updates are available.
