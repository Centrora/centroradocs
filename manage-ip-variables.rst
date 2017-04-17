Manage IPs and Variables
**************************

After the firewall is turned On, the IP records will be logged in the menu ``Logs --> Web Attacks``.

IP Status
--------------

An IP record can have 3 states, **Whitelisted**, **Blacklisted**, and **Monitored**.
* **Whitelisted** (marked as a green check) means the IP will not be scanned by the Firewall core engine;
* **Blacklisted** (marked as a red stop symbol) means the IP will be thoroughly blocked from the site and receive the block message;
* **Monitored** (marked as a yellow eye) means the IP is only logged in IP Management for the admin attention and the IP will still have access to the site.

Manage IPs
--------------

We can also manage the IPs in the same menu with the functional buttons.

* **Add IP**: It can add new IP rule to define new IP or IP range whitelist and blacklist. In the IP RuleTitle field, you can input anything which can remind you of the reason for adding the rule.
* **Blacklist IPs/Whitelist IPs/Monitor IPs**: You can use these buttons to switch between different IP states for a chosen IP.
* **Delete Items/Clear All Items**: To delete some or all existing IP rules in the IP Management.
* **Update Host**: To keep the host information of the IP up to date.
* **Import/Export IP from/to CSV**: The tool for importing or exporting IP rules.

Check IP record details
-------------------------------------

Generally we need to check the IP record details to find the reason for being logged in IP Control to judge if it’s a real hacking attack or a false alert, especially when you just start using the Firewall system. Based on the detailed information, you can whitelist the false alerted variables to make the system fit your site’s functions and make it more stable. To do this, please click on Action following an IP to review the details first.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/311_IP_List.jpg

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/312_IP_Details.jpg

As the screenshot shows, you can find two important values ``Detected Variable`` and ``Detected Content``. From the example of test with index.php?a=%27union, the variable is “get.a” and the blocked content is “union”. You can know it's a hacking attack from the blocked content. If the content is some legitimate text, for example you submit some text in the article which contains a sensitive word falsely alerted, you need to set the IP as “Monitored” and also whitelist the Variable in Variables Management to avoid it happening again in the future.

Whitelist variables
------------------------------------------

When you believe an IP is falsely logged and the variable is frequently falsely alerted, you can whitelist the variable in Variables Management. Go to the menu ``Firewall Setting --> Variables Fine-tuning``. Let’s still take the above test as example and assume it's a false alert. You can find all existing logged variables there and locate the one which we are going to whitelist based on the variable value “a”. Choose the variable and use the “Ignore the Variable” button to whitelist it.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/313_Whitelist_Variable.jpg

In the Variables Management section, each variable also has 3 possible states to choose from.

* **Scan the Variable**: It means the Firewall engine will actively scan for the variable’s content and block the IP if it violates the Firewall rules.
* **Filter the Variable**: It means the Firewall engine will still scan the variable’s content and log any suspicions, but it will not block the IP. This it for cases in which you are not sure whether the variable needs to be whitelisted and want to collect more information.
* **Ignore the Variable**: This means the variable is thoroughly whitelisted and the variable’s content will not be scan any more.

Load default whitelist variables
------------------------------------------------------------------

We strongly recommend you to load the default whitelist variables to reduce the number of false blocks for a normal website.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/314_Load_Default_Variables.jpg