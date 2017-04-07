Fatal error: Class PDO not found
************************************


If you encounter the error ``Fatal error: Class 'PDO' not found`` when the OSE Firewall is activated, this indicates the Class 'PHP Data Objects' is not loaded in your PHP environment. PDO is activated by default as of PHP 5.1.0, so please contact your hosting company to enable it if it is disabled.

.. Reference:: 'http://www.php.net/manual/en/pdo.installation.php <http://www.php.net/manual/en/pdo.installation.php>'_

If you know how to customize the php configuration, please edit the php.ini file, and add the following activation codes into it, that will resolve the issue:

1
2

extension=pdo.so

extension=pdo_mysql.so

Once the PDO is added to the php environment, issue will be resolved.