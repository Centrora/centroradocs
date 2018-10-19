Configure Firewall Settings of Centrora Version 6
****************************

Enable Centrora Firewall
-------------------------

Now, we can turn On Centrora Firewall to protect the website from attacks. Go to the menu ``Firewall Settings --> Firewall Configuration``, under the tab ``Firewall Scanning``, turn on ``firewall``. Setting it off will disable the Firewall scanning functions temporarily for the development purpose.

.. image:: https://cdn.centrora.com.au/images/Tutorials/300_Firewall_Scanning.jpg

Also, if you have Premium activated, please further go to the tab ``Advanced Firewall Configuration`` to enable ``Advanced Firewall Setting`` and ``Silent Mode``. The Advanced Firewall Setting is the switch of the advanced functions and features. It has more secured patterns and rules to help preventing all aspects of XSS attacks, sql injection etc. It will be only available for paid premium subscribers.

.. image:: https://cdn.centrora.com.au/images/Tutorials/301_Advanced_Firewall_Configuration.jpg

Frontend Blocking Mode
------------------------

1. There are 2 modes here. With **Show ban page**, if the user's behavior violates any rule, the user’s IP will be thoroughly blocked and they will receive a Ban Page which you can edit below.

2. The **Show a 403 error page** function allows a certain user's activity to be filtered, but the user’s IP will not be blocked and will just receive a 403 error page. Afterwards, the user can still get back to the site.

.. note:: We will recommend the mode of **Show a 403 error page**, in case the Firewall triggers false alerts. Banning the visitors' IPs may frustrate legitimate users.

3. **Silent Mode** in the ``Advanced Firewall Configuration`` is also recommended. It works with the v mode above. Under this mode, if an activity is recognized as hacking by Anti-Hacker, the user will be redirected to the URL with the suspicious string trimmed. Though the IP will not be blocked it will have been added to the monitored IP list. Thus, users will not be confused when their operations are falsely recognised as hacking activities.

4. Even under the mode of **Show a 403 error page**, we have the option to block the IP which keeps violates the rules and is considered belonging to a real hacker. **Silent Mode Allowed Threshold** in the ``Advanced Firewall Configuration`` defines the max number of suspicious visits of an IP. The default value is “10”.


Administrator Settings
------------------------

1. In the tab ``Administrator settings`` we can define the email address that will receive email alerts about Firewall activities.

2. **Centrora Google Authenticator**. This function is to unblock the administrator IP if it's falsely blocked. After enabling it, please scan the barcode with the Google Authentication App on our mobile. Also, there will be a field on the front-end ban page.

.. image:: https://cdn.centrora.com.au/images/Tutorials/302_Ban_Page.jpg

Whenever your admin IP is blocked out, you can access the Google Authentication App on your mobile to get the code. After submitting the code there, your IP will be immediately whitelisted and you will get the website access back.

Ban Page SEO
-------------------

Edit SEO to make the Firewall SEO friendly in case the search engine indexing/crawling is filtered/blocked/affected. For example, if a Google crawler is blocked, it might not detect website data and show website information in the search result correctly. In this case, the Firewall will send SEO information that you have set here to Google. However, please note that this is only a temporary solution and the best way is to find out the reason of the false blocks and to whitelist the related rules or variables which cause the false alarms.

If parameter is set as OFF for search engine (Google, Yahoo, and MSN) bots, the Firewall will bypass all visits from the specific search engine, hence there will be no false blocks for that search engine. Nevertheless, it is worth noting that there is a small potential risk here. Our past experience has observed that some hackers can disguise their IPs and activities to make them look like from Google bots. Bypassing Google bots will allow the access of this kinds of hackers.

Country Blocking
-------------------

This function allows you to block IPs from the specific countries. Please note that you need to download Country Database under the menu ``Firewall Settings --> Country Blocking`` before the function can be used.

.. image:: https://cdn.centrora.com.au/images/Tutorials/303_Download_Country_Date.jpg

After downloading the data, the full list of countries will be shown. You can choose a country and use the Blacklist Country to block visits from a specific country.

.. image:: https://cdn.centrora.com.au/images/Tutorials/304_Country_List.jpg

Brute Force Protection
-----------------------------

With the function enabled, a user’s account will be blocked when the maximum number of login attempts is reached within a given time period.

.. image:: https://cdn.centrora.com.au/images/Tutorials/305_Bruteforce.jpg

Google 2-Step Verification
----------------------------------

2-Step Google Authentication is only available for the WordPress and Joomla! currently. This function guarantees login security of a much higher level. Before the settings, you will need to install the Google Authenticator App on your mobile.

First, enable **Google 2-Step Verification** in the tab ``Brute Force Protection``.

Then for Joomla!, please go to the menu ``Users --> Manage``, edit the profile for the admin user in the tab ``Two Factor Authentication``. Set Authentication Method as **Google Authenticator** and follow the steps there to finalize the setup.

.. image:: https://cdn.centrora.com.au/images/Tutorials/306_Authentication_Joomla.jpg

For WordPress, please go to the menu ``Users`` and edit the admin account. In the section **Google Authenticator Settings**, set it Active. Click **Show/Hide QR code** to have the barcode showing and scan it with the mobile. Save the settings.

.. image:: https://cdn.centrora.com.au/images/Tutorials/307_Authentication_WP.jpg

After this is set, the google authenticator app from your smart phone will generate a code every minute, which makes your login highly secure. Even if a hacker knows your username and password, he will not able to access the site administrator area without the google authenticator code.

.. image:: https://cdn.centrora.com.au/images/Tutorials/308_Authentication_Login.jpg

Load Firewall Rules
--------------------

After the setting is done, please double check the firewall rules are loaded. Please go to menu ``Firewall Settings --> Firewall Rules Fine-tuning``. In ``Advanced Firewall Rules``, there is a button showing Firewall Update allowing you to do a manual update, if you have subscribed to our premium service. Thereafter, the Rules will be automatically updated.

.. image:: https://cdn.centrora.com.au/images/Tutorials/309_Advanced_Firewall_Rules.jpg


The configuration is all done. Your sites are now under protection by the firewall system.