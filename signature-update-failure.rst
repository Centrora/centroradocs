Signature Update Failure
**************************

If you come across Error of update database failure when updating the Signature or the Virus patterns, please check the below paths and set the permission of the folders into “777”.

For CentroraJoomla! version or Centrora Suite,
::

   /administrator/components/com_ose_firewall/protected/data
   /administrator/components/com_ose_firewall/protected/data/tmp
   /administrator/components/com_ose_firewall/protected/data/vsscanpath

For WordPress version,
::

   /wp-content/plugins/ose_firewall/protected/data
   /wp-content/plugins/ose_firewall/protected/data/tmp
   /wp-content/plugins/ose_firewall/protected/data/vsscanpath

If the Virus Signature date in Dynamic Scanner stays as an old date, please try to remove the file:

For Joomla!,
::

   /wp-content/plugins/ose-firewall/protected/data/tmpLastVersionCheck.php

For WP,
::

   /administrator/components/com_ose_firewall/protected/data/tmpLastVersionCheck.php

Then go back to the Dynamic Scanner and refresh page. The updater should reload again.
