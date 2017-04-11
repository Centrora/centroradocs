.. _track-file-change:

Track the File/Directory Change Time
**************************************


We sometimes observe that some specific files/directories keep being hacked. There is always because there are hidden codes in the website or some extensions have vulnerabilities. In this case, we need to find our the codes location which hack the know files.

First, we need to know the **exact date/time** of the file being modified. Please note this it not the modified time which we can find through the FTP. It's because the hacking codes may be able to change the file modified date shown in FTP to hide the useful information.

Then, we can check the **server raw access logs** for the records around the above exact change time to find our what files/commands did it.

Case 1: the specific file keeps being hacked.
---------------------------------------------

We need to get a notification when the file is hacked again and we use the script to achieve this. For example, the file is at ``/home/xxx/public_html/test.php``. Clean the file first. Then we get the latest modified date/time of the file by run a PHP file containing the codes::

   <?php
     $time = filemtime("/home/xxx/public_html/test.php");
     echo $time;
   ?>

Run the file to get the time value, say ``1491806973``.

Create another PHP file ``modified.php`` and place the codes in it::

   <?php
     //#Check the modified date/time of the file:
     // File
     $file = "/home/xxx/public_html/test.php";
     $time = filemtime($file);
     if ($time != '1491806973')
     {
       $result = mail("sample@domain.com","File hacked","File changed again"."\nFile time: ".date("Y-m-d H:i:s", $time)."\nEmail time: ".date("Y-m-d H:i:s"));
       echo "Completed-".$result."<br>";
     }
   ?>


Here, replace ``sample@domain.com`` to your own email address.

Now, add the script ``modified.php`` to the server cron job to make it run every 3 minutes::

   wget -q -O /dev/null http://your_domain/modified.php

When it detects the file is changed again, it will send an notification to your email where the "Email time" is the latest changed time. If you want the script to stop running whenever it detects any change to reduce the duplicate emails, please rename the file after ``echo "Completed-".$result."<br>";`` with the codes to make it::

       echo "Completed-".$result."<br>";
       rename ("/home/xxx/public_html/modified.php" , "/home/xxx/public_html/modified.php.bk");


We can check the server raw logs around that time to find more useful information.

Case 2: a specific folder always has strange uploaded files.
---------------------------------------------

In this case, we need to know the time when the files are really uploaded. We will count the file number in the folder, keep monitoring the number and send notification when the number changes.

Run the below script the count the current file number of the clean folder::

   <?php
     // Directory
     $directory = '/home/xxx/public_html/test';
     // Returns array of files
     $files = scandir($directory);
     $count = count($files);
     echo $count;
   ?>


Say the number of files is 9. Create the new PHP file ``count.php`` as::

   <?php
     //#Check the change of file count of a directory:
     // Directory
     $directory = "/home/xxx/public_html/test";
     // Returns array of files
     $files = scandir($directory);
     $count = count($files);
     if ($count != 9)
     {
       $result = mail("sample@domain.com","File added","Directory changed again"."\nFile time: ".date("Y-m-d H:i:s", $time)."\nEmail time:    ".date("Y-m-d H:i:s"));
       echo "Completed-".$result."<br>";
       rename ("/home/xxx/public_html/count.php" , "/home/xx/public_html/count.php.bk");
     }
   ?>

Replace ``sample@domain.com`` to your own email address.

Add the script ``count.php`` to the server cron job to make it run every 3 minutes::

   wget -q -O /dev/null http://your_domain/count.php

When new files are uploaded to the folder, it will detect the change and sen the notification with the time. We can check the server logs to find out the location of the hidden uploader.