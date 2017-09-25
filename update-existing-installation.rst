Update Centrora Version on an Existing Installation
**************************************************************

For Centrora Security Suite Users
--------------------------------------------

The upgrade process is quite simple if you already have Centrora Security Suite installed on the server. There are several ways to upgrade it.

1. Login your Centrora Security Suite installation. On the Dashboard, it will automatically detect the new version from our update server. If it successfully detects a new version, an Upgrade button will show up and you can click on it to do the upgrade.

2. Sometimes, method 1 might not return a success result due to some communication issues between servers or server settings. In this way, we can try a semi-manual way to upgrade. Login Centrora first and go to the menu Management --> Extension Manager. In Install URL, enter the below URL and Install. ``https://github.com/Centrora/centrora-suite-update/archive/master.zip``
3. If both 1 and 2 fail, you might have to use the manual way to upgrade it. Please download the Upgrade Package first. Extract it and upload all contents to the server directory: ``/Centrora_Suite_Installation_Path/tmp/v7/``. Then come back to Centrora Panel, menu Management --> Extension Manager, and in Install Directory filed, enter the above upload path: ``/Centrora_Suite_Installation_Path/tmp/v7/`` to install.

For Centrora Security Joomla! Version Users
----------------------------------------------------------------------

Please go to Joomla! Extensions --> Install --> Install from URL, and use the link ``https://github.com/Centrora/centrora-joomla/archive/master.zip`` to do the installation.

For Centrora Security WordPress Version Users
----------------------------------------------------------------------

Please directly update it in the WordPress Plugins section.

