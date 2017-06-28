.. _restore-website-from-cloud:

Restore Website from Cloud
********************************

Centrora Git Backup with the cloud space provides a secure zone for the website backup. Even when the site is down or files are erased by the hacker, we can restore it from the cloud backup.

Download the Restore Script
----------------------------

Please download the restore from Cloud script `here <https://github.com/ShawnOSE/Centrora-Git-Restore/archive/master.zip>`_.

Instruction
------------

1- Upload the script package to the directory where you would like to restore the website from the GitLab backup, say /httpdocs/test/.

2- Run the script as::

   http://your_site_URL/test/git.php

3- It will show a very simple panel where you can input the GitLab backup package information.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/520_Git_Restore_Page.jpg

4- On the form, the Git URL can be found from your GitLab account. Go to the Personal projects menu in GitLab after login and go to the project which you want to restore.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/521_GitLab_Projects.jpg

On the project page, choose **HTTPS** and copy the link.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/522_Git_Package_Link.jpg

5- Then go back to the Git restore page. Fill the form and click `Restore from Git`. It will show the brief download progress. The download is complete when it shows **The git has been pulled successfully**. It will redirect to the database restoration page automatically.

6- Now check the target directory /test, and we can find all files have been there.

7- Next, we need to prepare a database (better to be an empty one) and manually enter the Database information into above "Restore Database" page. Then `Restore database`.

The restoration is done.