Centrora Git Backup
********************

Centrora Git backup provides the best ever experience on the website backup and restoration. The backup function becomes stable and efficient since Version 6.8. Some new features with Git Backup were released as well to make it easier to use and more helpful, for instance, the ability of define the custom commit title and the file changes tracking function.

Please follow the below steps to set it up and refer to the videos for how to enjoy all functions of Centrora Git backup

1. Initialize Git Backup
-------------------------

When you use Git Backup for the first time, it needs to initialise the database and function. If all requirement checks are fulfilled, the Dashboard of Git Backup will automatically show the button ``Enable GitBackup 'Now'``. Click the button and the system will do the first backup.

.. image:: https://cdn.centrora.com.au/images/Tutorials/500_Enable_Git_Backup.jpg

After it's done, it shows the result of the first backup. The first backup will be named as "Initial Local Backup:" by default. Take a Joomla! site as the example, the backup list each core directory of the root separately to ensure the stability.

.. image:: https://cdn.centrora.com.au/images/Tutorials/501_First_Backup.jpg

You can also check the video about how to enable Git Backup.

.. raw:: html

   <a href="https://www.youtube.com/embed/2xkX801_NNo" target="_blank">Initialize Git Backup</a>
   <p></p>

2. Make a New Backup
---------------------

Now we can make a new backup at any time. The backup will be much faster then the initial backup because the Git technology only track and commit the changes from the initial one. Click the button ``Create local backup`` to make a new backup and here we can name the backup.

.. image:: https://cdn.centrora.com.au/images/Tutorials/502_Create_Local_Backup.jpg

After it's done, the new backup will be added to the list. Please note that in the new backup,only the changed directories from the last backup are listed.

.. image:: https://cdn.centrora.com.au/images/Tutorials/503_New_Backup.jpg

.. raw:: html

   <a href="https://www.youtube.com/embed/pS7TRE4P9iA" target="_blank">Make a New Backup</a>
   <p></p>


3. Track the Website Changes with Git
----------------------------------------

With the Git backup, we can easily track all changed files from the last backup. Click the ``Information``button following a backup to have all changed files in the specific directory listed in a pop-out window.

.. image:: https://cdn.centrora.com.au/images/Tutorials/504_File_Changes.jpg

.. raw:: html

   <a href="https://www.youtube.com/embed/Y2oxouteI9A" target="_blank">Track Website Changes with Git</a>
   <p></p>

4. Restore the Website to a Previous Backup
--------------------------------------------------------

Rolling back the website to a previous status is every easy, generally in seconds. Click the `Restore` button of a backup to go back to it. It will pop out a window to confirm if you would like to restore the database as well.

* Close - It will close the pop-out window and do nothing.
* No - Only restore the file system to the previous backup while keep the database unchanged.
* Yes - It will restore both the file system and database to the previous state.

.. image:: https://cdn.centrora.com.au/images/Tutorials/505_Restore.jpg

5. Upload to Cloud
------------------------------------------------

The backup can be uploaded to Cloud so that you can keep the backup safely even when the server gets any problem. Now Centrora Backup integrates with GitLab which provides up to 10GB space for each repository. If you have multiple websites, it can create multiple repositories under the same account. The number of repositories is unlimited. Please create an account on `GitLab Website <https://gitlab.com/users/sign_in#register-pane>`_ first if you don't have a GitLab account yet.

.. image:: https://cdn.centrora.com.au/images/Tutorials/507_GitLab_Account.jpg

After the account is created, please to the ``Settings`` --> ``Account`` menu to get the information of **Username** and **Private Token**. These two values are used to login you account in Centrora, and also Username is very important to define the web link where you can access all your existing repositories.

.. image:: https://cdn.centrora.com.au/images/Tutorials/508_Private_Token.jpg

Now, go back to Centrora Git Backup page and login with the above account.

.. image:: https://cdn.centrora.com.au/images/Tutorials/506_Login_Cloud.jpg

If there are changes on teh website from the last backup, it will also ask you to create and name a new backup first. Then the upload will automatically start. After it completes, you can find the backup has been uploaded to your account on GitLab at: https://gitlab.com/users/**your_username**/projects.

.. image:: https://cdn.centrora.com.au/images/Tutorials/509_Repository.jpg

Now the website is backed-up successfully on both local and cloud with Git. You can rescue the website with the backup easily from any emergency. If your server crashes or the website is totally down and you need a complete restoration, please refer to the guidance of ":ref: `restore-website-from-cloud`".



