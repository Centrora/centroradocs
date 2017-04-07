Install Centrora on WHM Server
*******************************


We are glad to announce that the new WHM / cPanel addon has been released to help you speed up the installation of Centrora Security onto your WHM server. This can enhance the firewall protection for your server.

Please do the installation following the below steps. **Please note that the installation on WHN will need the SSH login.**

1. Create new account in WHM.
---------------------------------

Login WHM control panel, Search ‘Create Account’ in the search bar and create a new account for the Centrora Security Suite installation with a sub-domain.

.. note:: The user account name must NOT be "centrora". You can use other account names like "centrorasuite".

.. image:: https://cdn.centrora.com/images/tutorial/whm/CrXpfI.png

2. Create new database and user.
---------------------------------

Once the account is created, access the cPanel control panel for this new account, and go to the MySQL Database section to create a new database and user account for Centrora Security.

.. image:: https://cdn.centrora.com/images/tutorial/whm/lZlVli.png


3. Run Centrora WHM install script.
-----------------------------------

Now, please access the SSH server and run the script (in one line)::

   cd ~/ && wget https://raw.githubusercontent.com/Centrora/centrora-suite/master/administrator/manifests/whm/install.sh && sh install.sh

It will prompt the following dialogue asking you the path of the Centrora installation, please enter the path and the account. Take the above account name "centrorasuite" as the example, the path is ``/home/centrorasuite/public_html/`` and the account is ``centrorasuite``. The installation will be continued like this,

.. image:: https://cdn.centrora.com/images/tutorial/whm/i0X58W.png

4. Install Centrora Security Suite in the account.
---------------------------------------------------

The Centrora Suite files now have been downloaded to the user account "centrorasuite" which you have created previously. Access the Centrora installation page at: ``http://sub-domain_for_Centrora_account/installation/index.php`` and follow the installation wizard to complete it.

.. image:: https://cdn.centrora.com/images/tutorial/whm/DvcDlG.png

5. Activate the Premium.
-------------------------

After the installation is done, please login the system and activate the premium service in the menu ``My Premium``.

6. Centrora Security is loaded in WHM.
--------------------------------------

A new plugin "Centrora Security" will show up in the WHM side bar.

.. image:: https://cdn.centrora.com/images/tutorial/whm/xKEtUe.png

7. Activate the firewall protection.
--------------------------------------

Now, you can scan all websites under the server /home folder when you access Centrora Security inside WHM. To protect the websites/accounts in the server, we need to do one more step to load the firewall functions.

First, please enter Centrora and go to the menu ``Management --> Firewall Activation Codes``.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/018_Suite_Activation_Codes.jpg

Copy the codes there starting with ";Parameters". For the WHM installation, they are normally::

   register_globals=off
   safe_mode=off
   allow_url_fopen=off
   display_errors=off
   session.save_path='/tmp'
   disable_functions="exec,passthru,shell_exec,system,curl_multi_exec,show_source"
   auto_prepend_file= "/usr/local/lib/php/centrora/administrator/scan.php"

Add the codes to the WHM server php.ini file through php.ini editor. Now, we can do a test to confirm the protection works following: :ref:`test-protection`.

We are sure that the new WHM addon helps you a lot in enhancing the firewall protection of your dedicated server.