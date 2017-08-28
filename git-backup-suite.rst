Using Git Backup in Centrora Suite on WHM server
**************************************************

1. Pre-requisites
--------------------------------------

If it's the first time you use Git Back in Centrora Suite and the system has not been initiated, the screen will show as the screenshot when you enter Git Backup Panel.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/530_Git_Suite_Panel.jpg

Since centrora is installed at the server root, it needs the database access of the website in a specific account. In order to do so we need to initiate the account which will allow centrora to get the database access. Please click on the ``Initiate`` button next to the account and it will try to retrieve the database details within the account based on the website system, Joomla! or WordPress. Once Git has been initialized for an account, it will look like this,

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/531_Git_Suite_Initialize.jpg

Notice that after the initialization, the button next to the account name changes to ``Go to the Account`` which means the system is able to retrieve the database detail.

In case the system fails to retrieve the database detail it will show up a pop-out window allowing you to manually input the database info.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/532_Git_Suite_Database.jpg

After setting the database connection, the system will check if the server settings satisfy the requirements of running Git. It will show the detailed report if any requirement is not fulfilled.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/533_Git_Suite_System_Check.jpg

2. Make A Backup
---------------------------------------------

Once all the requirements are satisfied you will see screen like this:





This means that all the pre-requisites are satisfied and the system is ready to go.
When you use the gitbackup for the first time , you need to enable gitbackup which will back up your database and files, so click on the button Enable Gitbackup ’Now’. Once that’s done , the screen will display message like this :




Once the initialisation is completed, the page will redirect you to the backup  panel which displays a list of backups




Unlike traditional backup, Git does not show the backup history using just a file name, instead it shows a list of backups carried out over time. Thus, if you back up a website once , the backup history will show your number of entries instead of one as it backups the website folder by folder.

FUNCTIONALITIES
UNINSTALL GIT
 This will delete all the git files and the plugin will stop tracking for all the changes. Which implies that all your backup and the backup history will be deleted. If you have performed a cloud backup previously, it will dis-link the cloud account but the repository will still exist.
CREATE LOCAL BACKUP
    This feature will back up your database along with the files. Once the process is completed the system will have a snapshot of the files in the system
So, to create a local backup, click on the create local backup icon  and it will show a pop up like this :




enter the name of the backup so that it will be easier for you to recollect the purpose of the backup in the future and click backup now.

PUSH BACKUP TO THE CLOUD:
This feature will perform a local backup first in case if it detects new changes and will upload them to your cloud account on GitLab (The users have a limit of 10 GB of cloud space on GitLab)
Here are the instructions for setting up the cloud account with centrora:
step 1: click on the push backup to the cloud buttons:



The system will prompt you if you have a GitLab account or not, GitLab is a cloud service provider which allows the users to upload the git backups. It is essential that you create an account with GitLab first if you want to use the cloud backup services. Follow the prompts on the screen until you have your username and token ready to create a repo.
How to get private token:
1.	go to: https://gitlab.com/users/sign_in and sign in using your username and password
2.	check the top right corner on the screen and click on settings section:










3.	copy the private token form the account section:




Use this private token and username for creating a cloud repository for your website on GitLab



Once you provide the username and access token in the form, the system will setup a folder for the cloud backup on the GitLab and will upload the backup to the account. The upload may take some time if you are uploading the backup for the first time, the time to upload will be quite smaller in the next upload operations.

LOCAL BACKUP AND CLOUD BACKUP NOTIFICATION
    When you see a red dot next to the local backup and cloud backup, it basically means that the system has detected new changes and provides the user an option to back up the new changes.


ROLLBACK:
Git back allows you to restore files as well as database form specific backups. Here are the instructions to perform a rollback:
Step 1: choose the backup you want to rollback to (Tip: use the green symbol with letter i to view changes) and click on the red rollback icon

Step 2: The system will show you a message like this:
If you want to roll back the database to the chosen backup then please click on yes (It is not recommended to roll back up to an old database as you may be losing some changes)


step 3: If the rollback is completed successfully. The green tick icon will appear next to the backup id that you wanted to rollback to.
Important note: You cannot rollback to the backup with the name as Initial local backup - since that is the first backup and the system has no other backup to roll back to

BACKUP CONTROL PANEL/ ACCOUNTS LIST:
Here is a details explanation of the backup control panel


The purpose of the control panel is to provide the administrator accessibility to view status of accounts as well perform backups with just one click.


LIST OF TECHNICAL WORDS AND THEIR MEANING:
1.	Repository: This can be interpreted as a folder
2.	Enable Git: Let git know it should start tracking for changed in the files
3.	Version Control: Keep track of changes in files
