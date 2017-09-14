Install/Update on Joomla! Website
**************************

The installation of Centrora plugin in a Joomla! website is quite easy. Please follow the below steps. The method also works to update Centrora to the latest version when you already have Centrora installed.

**Step 1.**

Go to Joomla! administration installation page through Joomla! back-end --> menu ``Extensions`` --> ``Manage`` --> ``Install``. Then go to the tab ``Install from URL``.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/005_Joomla!_Install.jpg

**Step 2.**

Simply copy/paste the URL into the box::

    https://github.com/Centrora/centrora-joomla/archive/master.zip

and click ``Check and Install`` button.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/006_Joomla!_Install_from_URL.jpg

**Step 3.**

After we get the installation success message, let's go to the menu ``Components`` --> ``Centrora Security`` to enter Centrora. On Centrora Panel, we need to install the database at ``Management`` --> ``Install/Uninstall`` for the first time installation.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/007_Joomla!_Install_DB.jpg

**Step 4.**
Also, please make sure the Centrora System system plugin is enabled. You can enable it by clicking the ``Fix it`` button if you see the notice message in the above Management menu. Or you can go to Joomla! Plugins Management, Joomla! ``Extensions`` --> ``Plugins`` and search for "Centrora". Enable it.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/008_Joomla!_Enable_Plugin.jpg

Congratulations!. Now the installation is done and we can continue the configurations.

**Alternative Installation Method**

If you have any troubles installing it using the above way, like the failed connection to our server or memory limit, please try the manual way to install it.

1. Download the install package to your computer from your account section on our website or the direct link, `Centrora Joomla! Package <https://github.com/Centrora/centrora-joomla/archive/master.zip>`_
2. Extract the package "centrora-joomla-master.zip" on your computer.
3. After the extraction, you can get a folder "packages" and find two packs in the folder "plg_system_centrora.zip" and "com_centrora.zip".
4. Further, extract the pack "com_centrora.zip" on local and upload all files to the website ``/site_root/tmp/centrora`` folder through the FTP.
5. Install it in Joomla! ``Extensions`` --> ``Install`` --> ``Install from Folder`` and enter the absolute path of the above upload directory to the box.
6. Click ``Check and Install`` to start the installation.
7. Do the same steps for the pack "plg_system_centrora.zip".
8. Now it's done and please follow the previous Step 3 and Step 4 to finalize the installation.

Please don't hesitate to `contact us <https://www.centrora.com/support>`_ if there is still any problem there.