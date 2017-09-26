Fatal error: Class PDO
************************************

.. error:: Class PDO not found

If you encounter the error ``Fatal error: Class 'PDO' not found`` when the OSE Firewall is activated, this indicates the Class 'PHP Data Objects' is not loaded in your PHP environment. You can do a check to confirm if the class exists.

**1** Make a new php file in your site root directory with name ``check_pdo.php``.

**2** Put the below codes into the file::

   <?php
     if (extension_loaded('pdo')) {
     echo "PDO is installed.";
     } else {
     echo "PDO is NOT installed.";
     }
   ?>

**3** Run the script on the site through the URL: *http://your_site_domain/check_pdo.php* and it will show the PDO status.

PDO is activated by default as of PHP 5.1.0, so if it's disabled please contact your hosting company to enable it.

Reference: `http://www.php.net/manual/en/pdo.installation.php <http://www.php.net/manual/en/pdo.installation.php>`_

If you manage the server or know how to customize the PHP configurations, please edit the php.ini file to add the following codes into it::

   extension = pdo.so
   extension = pdo_mysql.so

Once PDO is added to the PHP environment, issue will be resolved.

.. error:: Connection failed:SQLSTATE[HY000] [2002] No such file or directory. Fatal error: Call to amember function prepare() on a non-object

If you encounter this error, it means the PDO MySQLsocket might be missing on your server. Please upload an ``info.php`` file to the server with the codes::

   <?php
     phpinfo();
   ?>

Run the script through: *http://your_site_domain/info.php* to check the server PHP settings.

Search for ``mysql.default_socket``,and you could find its value is  ``/var/run/mysqld/mysqld.sock``.

Then search for ``pdo_mysql.default_socket``. It always returns a different value, for example ``/tmp/mysql.sock``. This is where the problem is. This directory might be missing or un-writable. The solution is to edit your server PHP settings to define::

   pdo_mysql.default_socket = /var/run/mysqld/mysqld.sock

Or please contact your host for the help if you are not allowed to change PHP settings on the server.
