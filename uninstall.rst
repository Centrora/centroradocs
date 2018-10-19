Uninstall Centrora from the System
*************************************

In case that you want to thoroughly remove Centrora System from your site or server, please follow the steps below.

WordPress Version:
--------------------

1. Remove the tables and data from the database first in ``Centrora --> Management → Install/Uninstall``.
2. Disable it in WordPress Plugins.
3. Remove it.

.. image:: https://cdn.centrora.com.au/images/Tutorials/019_Uninstall.jpg

Joomla! Version:
-----------------

1. Remove the tables and data from the database first in ``Centrora --> Management → Install/Uninstall``.
2. Disable the Centrora plugin is Joomla! Plugins manager.
3. Uninstall the component ``OSE Firewall`` and plugin ``Centrora`` in Joomla! Extensions Management.

Centrora Suite Version:
-------------------------

1. Remove the tables and data from the database first in ``Centrora --> Management → Install/Uninstall``.
2. Deactivate the protection for your site by removing the activation codes from the .htaccess. php.ini, or index.php file. It depends on in which way you did the protection activation at the beginning.
3. Remove the Centrora folder from the server.
4. Remove the database for the Centrora installation in MySQL.