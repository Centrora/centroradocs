********************************************
Install Centrora Suite version on the server
********************************************
Centrora Security Suite is a standalone system which is installed like a separate site on the server if you have a shared host. It can be also installed at the Server Root for the Dedicated Server / VPS.

Before the installation, please make sure that:

    1. You have backed-up your current websites, including all files and database just in case there are any accidents!
 	2. You have created a database that is specific for the Security Suite and is different from the databases of any of your existing websites!
 	3. You are installing the Centrora Security into a folder that is different from any of your existing websites! Such as:
       /public_html/centrora/

Now let’s start.

1. Download the Centrora installation package from Centrora website.

    [Download Centrora](https://www.centrora.com/download/) --> Download Standalone Version.

2. Extract the downloaded package on your computer and upload the files to the folder which is for the Centrora installation via FTP, say /public_html/centrora/. Or, you can directly upload the downloaded ".zip" pack to the server and extract it directly via the control panel file management. Then the files will look like this on the server,
.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/009_Suite_Files.jpg" alt="Suite Files" width="900" />

3. Go to the Centrora installation page at http://your_domain/centrora/installation/index.php
.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/010_Suite_Install.jpg

4. Follow the steps to do the installation.

<b>5.</b> At Step 4: Database, enter the information of the new database which you just created for the Centrora installation.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/011_Suite_Database.jpg" alt="Suite Database" width="900" />

<b>6.</b> You can just click ‘Next’ and ignore the FTP Configuration if you don’t need it.

<b>7.</b> In the Configuration step, add your preferred site name for the Centrora system and also the admin account info.

<b>8.</b> Remove the installation folder in the final step. <strong>Please note:</strong> if you have trouble automatically removing the installation folder due to the file ownership or permission reason, you need to manually remove that folder, at the location like /public_html/centrora/installation.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/012_Suite_Remove_Installation.jpg" alt="Remove Installation Folder" width="900" />

<b>9.</b> We can load the back-end by clicking <strong>“Administrator”</strong> button and login the new Centrora system.<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/013_Suite_Login.jpg" alt="Suite Login" width="900" />

<b>10.</b> After login, please go to the menu “Management“ --&gt; “Install/Uninstall” and follow the warning message to finalize the database installation.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/014_Suite_Install_DB.jpg" alt="Install Database" width="900" />

11. Finally, please enable the plugin “System – Centrora Security Activation Plugin” in Plugin Manager under the Management Menu.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/015_Suite_Activate_Plugin.jpg" alt="Enable Plugin" width="900" />

Installation finished. Now Centrora Suite is ready to be at your service!