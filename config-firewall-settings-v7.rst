Configure Firewall Settings
****************************

Basic Firewall Settings
-------------------------

To enable the firewall and configure the basic settings, following the Wizard is recommend as is an easy way to go through all major settings, especially for new users. We suggest you to enable all parameters for the best protection.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/330_Firewall_Wizard.jpg

Firewall Mode
--------------------------

There are three modes when the firewall detects suspicious activities.

1. Blocking Mode [Premium User]
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Blocking mode uses the combination of attempt count and firewall sensitivity to determine whether to block a user or not. By default, the attempt counts are set to 10 and the firewall sensitivity is set to level "sensitive". In this case, when the front-end visitors trigger over 10 times of operations/queries which are detected by the firewall at the "sensitive" standard, the visitors' IPs will be blocked. To make the firewall stricter towards attackers, you can lower down the attempt count and increase the firewall sensitivity. Once the user is blocked, he/she will not be able to view the website and will only see the ban page.

This mode is recommended for users who want to keep a strict security standard and do not want any suspicions to access the website.

2. Filter Mode [Premium User]
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Filter mode works differently from Blocking mode and in a more friendly way for front-end users. This mode focuses more on filtering and cleaning malicious requests/queries instead of blocking the IPs thoroughly. Under this mode, all suspicious activities will be silently filter and are not able to enter the website, meanwhile, it will not block the user IPs to avoid the confusion for users who make false positives.

However, it is important to note that this mode will still block users who perform attacks including,
  1.	Spamming
  2.	Using malicious user agents
  3.	Malicious file uploads
  4.	Brute force

3. Logging Mode [Free User]
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Logging mode is specially applied for free users. In this mode, the system will only keep track of attacks and will not block the attacker nor filter the request. The attack information can be viewed in the IP management page. The logging mode will send the alert email to the administrator when an attack is detected, and manual actions are required to block the IPs that trigger attacks. If the website is frequently attacked, it's recommend to subscribe our premium service to have the above 2 mode available to automatically block attacks.

Brute Force Protection
--------------------------------------------------------------

.. note:: Brute Force protection needs to work with website system plugin to detect the user login, so it's not available for Centrora Security Suite. We will try to add this feature in the future version of Centrora Suite.

Brute Force will detect the failure times of user login. With the function enabled, a user's account will be blocked when the maximum number of login attempts is reached within a given time period.

Also, a two-step Google authentication can be setup in order to make the website back-end immune to brute force attacks. Please follow the steps below to set it up.

For Joomla
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Click on the ``ON`` button to switch it active in the Brute Force section -> Google Verification tab.
2. A pop-up message will be shown for the confirmation. Click to continue.
3. You will be automatically redirected to the user's profile page in Joomla User Management.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/331_Firewall_2_Step_Joomla_User.jpg

4. Go on User Profile, enter the Two factor authentication tab and choose **Google Authenticator** as the authentication mode.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/332_Firewall_2_Step_Joomla_User_Profile.jpg

5. You will need to scan the barcode using the Google Authenticator app on your mobile phone. After scanning the barcode, the app will generate a 6-digit code.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/333_Firewall_2_Step_Joomla_Authentication_Code.jpg

6. Return to Joomla! User Profile and fill this code in the step 3 of the same page.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials334_Firewall_2_Step_Joomla_Fill_Code.jpg

7. Once the code is validated, the setup is completed. The google authenticator app from your smart phone will generate a code every minute when you need to login, which makes your login highly secure. Even if a hacker knows your username and password, he will not able to access the site administration area without the google authenticator.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/335_Firewall_2_Step_Joomla_Login.jpg

8. **Now, it's very important to go back to the previous Centrora Panel page to SAVE the configuration.**

9. Please set the 2-step authentication for all admin accounts.

For WordPress
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. The same, click on the ``ON`` slider to enable in the Brute Force section -> Google Verification tab.
2. A pop-up message will be shown for the confirmation. Click to continue.
3. You will be redirected to the user's profile page in the WordPress User Panel.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/336_Firewall_2_Step_WP_User.jpg

4. Tick the "Active" box and scan the barcode using the Google Authenticator app on your mobile phone. After scanning the barcode, the app will generate a 6-digit code. Save the setting.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/333_Firewall_2_Step_Joomla_Authentication_Code.jpg

5. After this is set, the google authenticator app from your smart phone will generate a code every minute when you need to login, which makes your login highly secure. Even if a hacker knows your username and password, he will not able to access the site administration area without the google authenticator.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/337_Firewall_2_Step_WP_Login.jpg


Ban Page SEO
-------------------

Edit SEO in the menu ``Advance Settings`` --> ``SEO Configuration`` to make the Firewall SEO friendly in case the search engine indexing/crawling is filtered/blocked/affected. For example, if a Google crawler is blocked, it might not detect website data and show website information in the search result correctly. In this case, the Firewall will send SEO information that you have set here to Google. However, please note that this is only a temporary solution and the best way is to find out the reason of the false blocks and to whitelist the related rules or variables which cause the false alarms.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/338_Firewall_SEO.jpg

If parameter is set as OFF for search engine (Google, Yahoo, and MSN) bots, the Firewall will bypass all visits from the specific search engine, hence there will be no false blocks for that search engine. Nevertheless, it is worth noting that there is a small potential risk here. Our past experience has observed that some hackers can disguise their IPs and activities to make them look like from Google bots. Bypassing Google bots will allow the access of this kinds of hackers.

Country Blocking
-------------------

This function allows you to block IPs from the specific countries. Please note that you need to download Country Database under the menu ``Advance Settings`` --> ``Country Blocking`` before the function can be used.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/339_Firewall_Download_Country_Date.jpg

After downloading the data, the full list of countries will be shown. You can choose a country and make the shield icon to **Red** to block visits from a specific country. Moreover, if you set the shield as **green**, the country will not be scanned by the firewall and all IPs from the country can access the website without any monitor. A **yellow** means the country will be under the firewall's monitor normally.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/340_Firewall_Country_List.jpg

