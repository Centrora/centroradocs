Fatal error: Class PDO not found
************************************


If you encounter the error ``Fatal error: Class 'PDO' not found`` when the OSE Firewall is activated, this indicates the Class 'PHP Data Objects' is not loaded in your PHP environment. You can do a check to confirm if the class exists.

1. Make a new php file in your site root directory with name ``check_pdo.php``.
2. Put the below codes into the file::

   <?php
     if (extension_loaded('pdo')) {
     echo "PDO is installed.";
     } else {
     echo "PDO is NOT installed.";
     }
   ?>

3.

PDO is activated by default as of PHP 5.1.0, so please contact your hosting company to enable it if it is disabled.

Reference: `http://www.php.net/manual/en/pdo.installation.php <http://www.php.net/manual/en/pdo.installation.php>`_

Or you can do a check

If you know how to customize the php configuration, please edit the php.ini file, and add the following activation codes into it, that will resolve the issue:

1
2

extension=pdo.so

extension=pdo_mysql.so

Once the PDO is added to the php environment, issue will be resolved.