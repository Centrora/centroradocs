Using Git Backup in Centrora Suite on WHM server
**************************************************

1. Pre-requisites
--------------------------------------

If it's the first time you use Git Back in Centrora Suite and the system has not been initiated, the screen will show as the screenshot when you enter Git Backup Panel.

.. image:: https://cdn.centrora.com.au/images/Tutorials/530_Git_Suite_Panel.jpg

Since centrora is installed at the server root, it needs the database access of the website in a specific account. In order to do so we need to initiate the account which will allow centrora to get the database access. Please click on the ``Initiate`` button next to the account and it will try to retrieve the database details within the account based on the website system, Joomla! or WordPress. Once Git has been initialized for an account, it will look like this,

.. image:: https://cdn.centrora.com.au/images/Tutorials/531_Git_Suite_Initialize.jpg

Notice that after the initialization, the button next to the account name changes to ``Go to the Account`` which means the system is able to retrieve the database detail.

In case the system fails to retrieve the database detail it will show up a pop-out window allowing you to manually input the database info.

.. image:: https://cdn.centrora.com.au/images/Tutorials/532_Git_Suite_Database.jpg

After setting the database connection, the system will check if the server settings satisfy the requirements of running Git. It will show the detailed report if any requirement is not fulfilled.

.. image:: https://cdn.centrora.com.au/images/Tutorials/533_Git_Suite_System_Check.jpg

2. Enable the Backup
---------------------------------------------

Now we can enable Git Backup if all requirement checks pass and it shows the successful window.

.. image:: https://cdn.centrora.com.au/images/Tutorials/534_Git_Suite_Enable_Backup.jpg

It will automatically start the first backup of the files and database.

.. image:: https://cdn.centrora.com.au/images/Tutorials/535_Git_Suite_Backup.jpg

Once the initialization is done, the page will redirect you to the main backup management panel which displays the list of all backups of the account.

.. image:: https://cdn.centrora.com.au/images/Tutorials/536_Git_Suite_Backup_List.jpg

Unlike the traditional backup method, Git backup will not show the backup history which includes a list of packages each for a whole website backup. Instead it shows a list of backups carried out over time each only tracking the changes from the previous backup.

3. Uninstall Git
---------------------------------------------

This will delete all Git files and the plugin will stop tracking for all the changes. Then all your backups and the backup history will be deleted. If you have performed a cloud backup previously, it will dis-link the cloud account but the repository will still exist in the cloud account.

4. Create Local Backup
---------------------------------------------------------------

This will make a backup of the site database and the files. Once the process is completed the system will have a snapshot of the files in the system. After clicking on the ``Create local backup`` icon , it will show a pop up like this :

.. image:: https://cdn.centrora.com.au/images/Tutorials/537_Git_Suite_Create_Backup.jpg

Here you can name the current backup to remark the purpose of the backup.

5. Push Backup to cloud
--------------------------------------------------------------

This feature will perform a local backup first and then upload it to your cloud account on GitLab. Please note that to use this feature, you might need to control the website size under 10GB as each repository with GitLab has a limit of 10 GB of cloud space.

Please refer to the tutorial `Upload Git Backup to CLoud <https://docs.centrora.com/en/latest/git-backup.html#upload-to-cloud>`_

6. Backup Notification
-----------------------------------------------------------------

When the red dots next to the local backup and cloud backup are shown as in the previous screenshot, it basically means that the system  detects new changes and suggests the admin to backup for the new changes.

7. Backup Control Panel / Accounts List for WHM Accounts
----------------------------------------------------------------------

The purpose of the control panel is to provide the administration accessibility to view the status of backups of different accounts and perform backups directly without entering each account.

.. image:: https://cdn.centrora.com.au/images/Tutorials/539_Git_Suite_Account_List.jpg
