Install Centrora on WHM Server
*******************************


We are glad to announce that the new WHM / cPanel addon has been released to help you speed up the installation of Centrora Security onto your WHM server. This can enhance the firewall protection for your server.

Please do the installation following the below steps. **Please note that the installation on WHN will need the SSH login.**

1. Create new account in WHM
---------------------------------

Login WHM control panel, Search ‘Create Account’ in the search bar and create a new account for the Centrora Security Suite installation with a sub-domain.

.. note:: The user account name must NOT be "centrora". You can use other account names like "centrorasuite".

.. image:: https://cdn.centrora.com/images/tutorial/whm/CrXpfI.png

2. Create new database and user
---------------------------------

Once the account is created, access the cPanel control panel for this new account, and go to the MySQL Database section to create a new database and user account for Centrora Security.

.. image:: https://cdn.centrora.com/images/tutorial/whm/lZlVli.png


3. Run Centrora WHM install script
-----------------------------------

Now, please access the SSH server and run the script (in one line)::

   cd ~/ && wget https://raw.githubusercontent.com/Centrora/centrora-suite/master/administrator/manifests/whm/install.sh && sh install.sh

It will prompt the following dialogue asking you the path of the Centrora installation, please enter the path and the account. Take the above account name "centrorasuite" as the example, the path is ``/home/centrorasuite/public_html/`` and the account is ``centrorasuite``. The installation will be continued like this,

.. image:: https://cdn.centrora.com/images/tutorial/whm/i0X58W.png

4. Install Centrora Security Suite in the account.

The Centrora Suite files have been downloaded to the user account "centrorasuite" which you have created previously. Access the Centrora installation page at: ``http://sub-domain_for_Centrora_account/installation/index.php`` and follow the installation wizard to complete it.




After the database is created, access the File Manager and browse the ‘public_html’ folder, click the ‘Upload’ button to upload the Centrora Security Suite package.</li>
</ol>
<img class="aligncenter" src="https://cdn.centrora.com/images/tutorial/whm/tO78Ct.png" alt="Firewall Protection" width="604" height="207" />

<img class="aligncenter" src="https://cdn.centrora.com/images/tutorial/whm/Hx3swG.png" alt="Firewall Protection" width="610" height="275" />

Then extract the zip package, and access the Centrora Installation page:

<img class="aligncenter" src="https://cdn.centrora.com/images/tutorial/whm/DvcDlG.png" alt="Firewall Protection" width="612" height="280" />

Follow the installation wizard to fill in the required information and completed the installation.

Note: When completed, please <strong>activate the premium service before continue</strong> to setup the WHM firewall protection in the following steps. To do so, please go to Centrora Security --&gt; My Account --&gt; Login with your email address and password --&gt; Activate the premium service.

4. Have you activated the premium service? If so, move on:

After that, login your SSH server, and run the following commands:
<pre class="lang:php decode:true">mkdir ~/centrora
cd ~/centrora
wget http://www.centrora.com/downloads/install.zip
unzip install.zip
sh install.sh</pre>
5. You will prompt the following dialogue asking you the path of the Centrora installation, please enter the path, e.g. /home/centrorasuite/public_html/, the installation will be continued like this

<img class="aligncenter" src="https://cdn.centrora.com/images/tutorial/whm/i0X58W.png" alt="Firewall Protection" width="799" height="279" />

&nbsp;

6. When completed, you will see Centrora Security in the WHM side bar:
<img class="aligncenter" src="https://cdn.centrora.com/images/tutorial/whm/xKEtUe.png" alt="Firewall Protection" width="808" height="370" />

&nbsp;

You can now scan all websites under the /home folder when you access Centrora Security inside WHM. We are sure that the new WHM addon helps you a lot in enhancing the firewall protection of your dedicated server.