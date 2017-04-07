.. _test-protection:

Test Firewall Protection
***************************

After enabling the Firewall, we need to have a test to make sure it works to protect the website.
We can test the Centrora Firewall function using the URL:


http://your_site_URL/index.php?a=%27union
1
http://your_site_URL/index.php?a=%27union
Then you will be blocked if you set the protection mode as “Ban IP” mode in Firewall Configuration menu –> Firewall Configuration.

(We suggest you to set it as “Ban IP mode” mode when doing the test as it will show the result clearly. After the test, please set it back to 403 mode and also turn on Silent Filter Mode in Advanced Firewall Configurations).

If the test doesn’t return the expected result, it means the activation might not be successfully done. The server might have some special settings. Please contact your host with the question, How to have a local custom PHP configuration setting; or please feel free to contact us at our Support Center.