.. _test-protection:

Test Firewall Protection
***************************

After enabling the Firewall, we need to have a test to make sure it works to protect the website.

First, please we suggest setting it as "Ban Page" mode in the ``Firewall Configuration`` before doing the test and disable the "Advanced Firewall Setting" as it will show the result clearly. After the test, please set it the firewall setting back to 403 mode and also turn on Silent Filter Mode in Advanced Firewall Configurations to make sure the firewall works smoothly.

We can test the Centrora Firewall function using the URL::

   http://your_site_URL/index.php?a=%27union

Then you will be blocked with the block page showing up.

If the test doesn't return the expected result, please check if you have ModSecurity installed on the server if you manage the server. ModSecurity may filter the testing query first. If not the case, it means the protection is not enabled well. Please `contact us <https://www.centrora.com/support>`_ at our Support Center for help.