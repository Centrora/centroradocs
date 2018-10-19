Install Centrora on Plesk Server
*******************************


We have released the installation method specific for the Plesk Server. This can enhance the firewall protection for your Plesk server.

Please do the installation following the below steps. **Please note that the installation on Plesk will need the SSH login.**

1. Create new account in Plesk.
---------------------------------

Login Plesk control panel, in "Domains" add a new domain for the Centrora Security Suite installation, like suiteplesk.your_domain.com.

.. note:: The user account name must NOT be "centrora". You can use other account names like "suiteplesk".

.. image:: https://cdn.centrora.com.au/images/Tutorials/031_Plesk_Account.jpg

2. Create new database and user.
---------------------------------

Once the domain is created, access its management panel, and go to "Database" section to create a new database and user account for Centrora Security.

.. image:: https://cdn.centrora.com.au/images/Tutorials/032_Plesk_Database.jpg

3. Upload Centrora Suite files.
-------------------------------------------------

Download the Centrora Suite version from the website: `https://www.centrora.com/download/ <https://www.centrora.com/download/>`_ --> Download Standalone version. Upload the package  to the previous domain path in Plesk --> Manage the domain --> File Manager.

.. image:: https://cdn.centrora.com.au/images/Tutorials/033_Upload_Package.jpg

Then extract the package and it will create a new folder ``centrora-suite-master``. Enter the folder and move all files there to the root (httpdocs).

.. image:: https://cdn.centrora.com.au/images/Tutorials/034_Move_Files.jpg

4. Install Centrora Security Suite in the account.
---------------------------------------------------

Now we can access the Centrora installation page at: ``http://domain_for_Centrora_account/installation/index.php`` and follow the installation wizard to complete it. After the installation, login and install the database.

.. image:: https://cdn.centrora.com/images/tutorial/whm/DvcDlG.png

5. Activate the Premium.
-------------------------

After the installation is done, please login the system and activate the premium service in the menu ``My Premium``. Please also refer to: :ref:`activate-premium`.

6. Run Centrora Plesk install script.
-----------------------------------

Now, please access the SSH server and run the script (in one line)::

   cd && mkdir centrora && cd centrora && wget https://raw.githubusercontent.com/HelixLee/centrora-plesk/master/install.sh && chmod +x install.sh && sh install.sh

It will automatically create the extension in Plesk --> Extensions.

7. Sync files from the local account to the global location.
-----------------------------------------------------------------------

Run the commands in SSH,::

   cd /usr/local/psa/admin/htdocs/modules/centrora
   rm -rf installation
   rsync -rv /var/www/vhosts/suiteplesk.your_domain.com/httpdocs/* /usr/local/psa/admin/htdocs/modules/centrora
   chown psaadm:psaadm -R /usr/local/psa/admin/htdocs/modules/centrora

In the above code, please replace **suiteplesk.your_domain.com** with the real domain for Suite installation created in Step 1.

8. Centrora Security is loaded in Plesk.
--------------------------------------

A new extension "Centrora Security" will show up in Plesk Extensions menu.

.. image:: https://cdn.centrora.com.au/images/Tutorials/035_Extensions.jpg

We can access Centrora Security and do the management through this portal in teh future.

9. Edit the configuration.
-----------------------------------------

Now we need to update the /tmp and /log paths of the Centrora installation. Login Centrora from Plesk Extensions and go to the menu ``Management`` --> ``Global Configuration``. Change "Path to Log Folder" as::

   /usr/local/psa/admin/htdocs/modules/centrora/logs

and change "Path to Temp Folder" as::

   /usr/local/psa/admin/htdocs/modules/centrora/tmp

Save the settings.

10. Activate the firewall protection.
--------------------------------------

Now, we can scan all websites under the server /var/www/vhosts folder when we access Centrora Security inside Plesk. To protect the websites/accounts in the server, we need to do one more step to load the firewall functions.

First, please enter Centrora and go to the menu ``Management --> Firewall Activation Codes``.

.. image:: https://cdn.centrora.com.au/images/Tutorials/036_Plesk_Activation_Code.jpg

Copy the codes::

   auto_prepend_file= "/opt/psa/admin/htdocs/modules/centrora/administrator/scan.php"

and insert the line into the ``PHP Settings`` of the domain which we are going to protect.

.. image:: https://cdn.centrora.com.au/images/Tutorials/037_Insert_Activation_Codes.jpg

Also, add the path::

   /opt/psa/admin/htdocs/modules/centrora

into the parameter ``open_basedir``.

.. image:: https://cdn.centrora.com.au/images/Tutorials/038_open_basedir.jpg

Now, we can do a test to confirm the protection works following: :ref:`test-protection`.