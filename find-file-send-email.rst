Find File Sending Emails
**************************

We might observe spam emails are sending from our server. However, it's very hard to locate the scripts which send them. Here we can have a method to track their locations if we can define a local PHP configuration on the server.

First, we need to define these 2 parameters in the PHP configuration. For example, on your server, the websites is located in the directory ``/home/doamin/public_html``, define::

    mail.add_x_header = On
    mail.log = /home/doamin/public_html/phpmail.log

It could be a php.ini file on your server. Please make sure it's the loaded PHP configuration of all scripts on the server.

Then we can do a test. Upload a ``test.php`` to the site ``/tmp`` directory. Add the PHP codes to the file::

    <?php
    // the message
    $msg = "First line of email body\nSecond line of email body";

    // use wordwrap() if lines are longer than 70 characters
    $msg = wordwrap($msg,70);

    // send email
    mail("Jack@test.com","Test Email",$msg);
    ?>

Run the test file at *http://your_site_domain/tmp/test.php*. If the email is sent, it will be logged in the ``phpmail.log`` file which we defined previously::

   [06-Oct-2016 01:38:43 America/Chicago] mail() on [/home/domain/public_html/tmp/test.php:9]: To: Jack@test.com -- Headers:

Here we can find the file location which sends the email. After setting all these, we can check the mail log file next day. We can then know all files sending emails during the period.