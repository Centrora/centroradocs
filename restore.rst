Restore Website from Cloud
********************************

Centrora Git Backup with the cloud space provides a secure zone for the website backup. Even when the site is down or files are erased by the hacker, we can restore it from the cloud backup.

Download the Restore Script
----------------------------

Please download the script at [https://github.com/ShawnOSE/Centrora-Git-Restore/archive/master.zip](https://github.com/ShawnOSE/Centrora-Git-Restore/archive/master.zip)

Instruction
------------

1- Upload the script package to the directory where you would like to restore the website from the BitBucket backup, say ``/httpdocs/test/``.

2- Run the script as http://your_site_URL/test/git.php

3- It will show a very simple panel where you can input the BitBucket account information.

.. image:: https://cdn.protect-website.co/centrora_web/images/Community/Centrora Git Restore/2017-03-21_07-59-18.png

4- In the form, the Git URL can be found from your BitBucket account. Go to the repository which you want to restore and you can get it from the browser address bar.

.. image:: https://cdn.protect-website.co/centrora_web/images/Community/Centrora Git Restore/2017-03-21_08-11-14.png

5- Then go back to the Git restore page and click `Restore from Git`. It will show the brief download progress. The download is complete when it shows **The git has been pulled successfully**.

6- Now check the target directory /test, and we can find all files have been there.

7- Next, we need to prepare a database (better to be an empty one) and manually enter the Database information into the website configuration file, **configuration.php** for Joomla!, and **wp-config,php** for WordPress.

8- Go back the Git restore page again and click ``Restore database``.

The restoration is done.