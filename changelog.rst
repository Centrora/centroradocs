Changelog
*****************************************

7.0.2

* Minor bug fixes for firewall scanner v7.
* Minor bug fixes for core directory scanner.
* Added new hash files.
* Added missing language tags.
* Fixed Wordpress centrora security badge.
* Fixed cron job page to include git backup pre-requisite checks only when the user want to change the scheduled git backup settings.
* Added new OEM.
* Fixed links to update the plugin version

7.0.1

* Fixed missing v7 firewall file issue

7.0.0

* Added new feature: new improved, faster and efficient Firewall v7 scanner.
* Use of high speed dedicated servers for virus scanning and Git backups.
* Removal of classic backup.
* Improved Git Backup which supports increased cloud backup space of 10 GB.
* Improved the feature to update the virus and firewall patterns.
* Improved efficiency of MD5 hash scanner, core directory scanner, vulnerability scanner and file permission scanner.
* Improved manual and schedule scanning.
* Minor bug fixes for Firewall scanner V6.

6.6.4.1

* Fixed: download function not working on some websites
* Fixed: PHP errors in php7.1.1
* Improved Email templates

6.6.4

* Added WordPress 4.7.1 and 4.7.2 hash files for core file scanning

6.6.3

* Updated email templates
* Improved virus scanning functions
* Improved firewall scanning functions when variables are iterated arrays

6.6.2

* Update Mailer class to remove Joomla version codes

6.6.1

* Remove PHPmailer and use Default WordPress PHPmailer to send emails

6.6.0

* Added new OEM
* Improved UI for all scanner sections
* Fixed Firewall Scanner bug when variable is an nested array
* Updated software update url to github url
* Fixed virus scanner bug for whitelisted files
* Plesk Panel support
* Update PHP Mailer to latest version

6.5.16

* Added WordPress 4.7 hashes files

6.5.15

* Fixed mark as clean doesn’t work correctly on schedule scanning issues

6.5.14

* Added WordPress 4.6.1 hashes for Core Directory Scanner

6.5.13

* Updated Backup function to check file permissions before performing actual backup

6.5.12

* Fixed minor warning errors when checking URLs for cronjob requests

6.5.11

* Fixed installer not working on Windows server due to the lack of INNODB engine

6.5.10

* Updated API IP address

6.5.9

* Improved Add IP function to cleanup IP title to enhance security, credits to ‘Plugin Vulnerabilities’

6.5.8

* Add administrator checking to improve AJAX security check function to enhance CSRF protection

6.5.7

* Improved AJAX security check function to enhance CSRF protection

6.5.6

* Fixed update error for French language websites

6.5.5

* Added French language package

6.5.4

* Fixed span tags not showing properly in malware detail popup
* Added French language support preparation package

6.5.3

* Added background scanning function

6.5.2

* Improved Malware scanner function
* Improved Database installation function to reduce database connections
* Added WordPress 4.5.3 hashes

6.5.1

* Improved Marked As Clean function in Virus scanner

6.5.0

* PHP 7 support
* Improved the efficiency of schedule virus scanner to
* Improved the efficiency of Gitbackup

6.4.3

* Improved Git Backup for large websites
* Fixed other minor UI bugs

6.4.2

* Fixed Git push to cloud name error

6.4.1

* Fixed Git push to cloud error

6.4.0

* Improved Gitbackup function
* Improved Gitbackup UI
* Improved Gitbackup cronjob
* Disable google bot user agent detect
* Improved: import csv file function in IP Management section
* Fixed: Scan result status filter not working properly on some websites
* Added WordPress 4.5.1 and 4.5.2 hash files

6.3.5

* Fix free virus scanning function not working properly on some servers

6.3.4

* Improved Gitbackup checking function

6.3.3

* Improved Virus Scanning report section UI

6.3.2

* Fixed IP import function not working properly when CSV file is modified in Windows Excel file
* Added IPv6 Support
* Improved Virus Scanning report section UI
* Improved firewall scanning report email by adding the link to the IP information page

6.3.1

* Fixed the blank header section in the configuration page
* Fixed some minor css issues.
* Fixed the scan report result link to the scan report in the WordPress version for Joomla versions

6.3.0

* Improve Cloud backup for Gitbackup
* Improve dynamic Virus scanner UI
* Added new schedule scanner function
* Fixed firewall rules update function not working on some servers
* Fixed Core directory scanner not working on some servers

6.2.4

* Fixed some css and javascript issues in the dashboard and Gitbackup UI

6.2.3

* Close error display

6.2.2

* Fixed error handling function not working properly on some servers for Gitbackup

6.2.1

* Added Git Backup error handling message if Git is not installed
* Added Git Backup folder protection

6.2.0

* Added Git Backup
* Improved User Interface

6.1.4

* Fixed IP Import not functioning after security token method is changed

6.1.3

* Fixed IP cannot be added and virus scanner cannot start for some websites after the token method changes

6.1.2

* Fixed IP curb and scanning report not showing up properly issues after the token method changes

6.1.1

* Fixed a low severity XSS vulnerability in backup file name function, credits to Erin Germ
* Fixed a low ot medium severity CSRF vulnerability when an article is posted by Editors with the form to manipulate the Centrora database, credits to Erin Germ

6.1.0

* Updated Core Directory Scanner
* Add more hashes for Joomla and WordPress previous versions

6.0.7

* Updated WordPress hash for 4.4.2

6.0.6

* Fixed bugs for Windows server
* Fixed directories not showing correctly in WHM installation for Core directory scanning
* Remove the scanning of Long queries (more than 255 characters)
* Fixed Vulnerabilities scanner showing com_contact as vulnerable for Joomla 3.4

6.0.5

* Fixed virus scanning report reloading to the 1st page if the current page is not in the 1st page

6.0.4

* Fixed scheduled virus scanner not working on some servers

6.0.3

* Fixed modified file scanner not working issue on some websites
* Fixed virus scanner report csv file not working properly on WordPress websites
* Fixed email template not showing properly when the save button is clicked the from the second time

6.0.2

* Harden the website by adding one rule to prevent remote execution vulnerability
* Fixed PHP notice message for advance firewall scanner
* Add Joomla remote code execution vulnerability protection
* Fixed virus scanner notice warnings
* Add function to block IPs with malicious user agents
* Add function to block IPs with fake google bots
* Updated Email template editing function

6.0.1

* Added more rules in checking malicious user agent
* Removed Google Authentication in Block page when the option is turned off
* Updated mail class
* Fixed configuration setting not saved successfully on some servers

6.0.0

* Added: Brand New Look and feel! – We took valuable feedback from you our customers and revamped the look of Centrora Security. Give it a go, we think you will love it!
* Added: Help text to give users a better understanding of each configuration setting
* Added: Strong Password Enforcement under Firewall configuration settings
* Added: A What’s New section where you can view News of security and other related posts from our own security consultants – learn what you can do to harden your site’s security
* Enhancement: Merge Firewall Configuration Functions
* Enhancement: Improved firewall configuration settings layout – Rearranged & simplified configuration settings
* Enhancement: Reduced duplicate functions under Firewall
* Enhancement: Improved site navigation speed
* Enhancement: Changelog view under what’s new to get details of each release

5.0.8

* Enhancement: Improve file upload function to have better user experience

5.0.7

* Enhancement: Hide errors for all situations
* Enhancement: Add extra protection on data folder

5.0.6

* Fixed: Language file not loaded properly for scheduled virus scanning.

5.0.5

* Fixed: The syntax for OEM version does not work in PHP version 5.3 that caused some websites not working properly
* Added: Administrator URL protection for both WordPress, Joomla and Suite versions
* Added: Security Manager Account management section to add a security manager account to manage Centrora Security
* Enhancement: Enhanced CSS and UI support for OEM partners
* Added: Security warning message in configuration page to enable the Centrora System plugin for Joomla and Suite users
* Bug fixed: Suite version only – fixed errors showing in the administrator menus
* Bug fixed: Suite version only – JFactory not found error when loading the language tags

5.0.4

* Added: Added file upload logging function for premium users
* Enhancement: Enhanced the panel for allowed file extensions for file uploads

5.0.3

* Fixed: Fixed the Firewall checking warning message shows incorrectly when the firewall is turned on

5.0.2

* Enhancement: Improve the virus scanner and scanner report to use stricter patterns to avoid false alerts

5.0.1

* Enhancement: Change the virus scanner to use stricter patterns during the scanning to avoid false alerts

5.0.0

* Added: Brand New Look and feel! – We took valuable feedback from you our customers and revamped the look of Centrora Security. Give it a go, we think you will love it!
* Added: Help text to give users a better understanding of each configuration setting
* Added: Strong Password Enforcement under Firewall configuration settings
* Added: A What’s New section where you can view News of security and other related posts from our own security consultants – learn what you can do to harden your site’s security
* Enhancement: Merge Firewall Configuration Functions
* Enhancement: Improved firewall configuration settings layout – Rearranged & simplified configuration settings
* Enhancement: Reduced duplicate functions under Firewall
* Enhancement: Improved site navigation speed
* Enhancement: Changelog view under what’s new to get details of each release
* Enhancement: Improved Dashboard design (Phase 1) – expect more to come!
* Fixed: Audit page fixes to “Fix” button
* Fixed: Other minor visual bug fixes
* Fixed: Minor JS fixes for data pagination

4.9.4

* Enhancement: improve firewall scanner to avoid an warning error when returning scanning results
* Enhancement: improve virus scanner to detect PHP injection scripts faster

4.9.3

* Fixed: Fixed firewall version not updated when using the Update Signature function
* Fixed: Fixed virus Pattern update was not successful for some servers when using the Update Virus Pattern function

4.9.2

* Enhancement: Improved the returned message after the firewall signature is updated.

4.9.1

* Fixed: Fixed the signature update function in Advance Firewall Panel
* Fixed: Fixed backup panel not showing up properly in some servers with PHP version lower than 5.4
* Fixed: Minor fix for Javascript functions
* Updated: updated the Danish language file

4.9.0

* Added: Add Google Drive backup
* Added: Feature Requests #91: Back up function Offer other Options for Low server memory constraint users
* Added: Support for larger file size uploads (cloud backup)
* Added: Feature Requests #124: Add manual update function in the admin backend
* Added: Feature Requests #167: Add download virus pattern function to virus scanner section
* Enhancement: Improved backup Upload time – Faster More efficient Cloud Backups.
* Enhancement: Split backups for manageable file sizes
* Enhancement: Backup option for timeout constraint servers (during files backup )
* : Improvements #119: Reorganise Menu System for better navigability
* Fix: Scheduled backup function fixes
* Fix: Bugs #85: Creating Backup Zip fails for some users
* Fix: Bugs #127: Premium Subscription multisite login Issues
* Fix: Bugs #161: Email template mass
* Fix: Minor UI fixes
* Fixed: Fixed warning error: “Undefined property: stdClass::$ischecked in fwscanner.php”

4.8.5

* Fixed: Fixed Quarantine file failed issue in Joomla component version

4.8.4

* Fixed: Ban IP page css not loaded properly for some websites

4.8.3

* Fixed: duplicated IP in IP management

4.8.2

* Enhancement: Improved firewall scanner class to remove miscellaneous warning errors
* Enhancement: Improved firewall management codes to avoid duplicated IP showing in the IP management section
* Enhancement: Added variable validation function on backup path variable in backup management section
* Enhancement: Improved Dropbox and One Drive Authentication function

4.8.1

* Fixed: Schedule Tasks hour selector saving the wrong time on the server.
* Added: Added email template restore function.

4.8.0

* Added: New and Improved Schedule Task: Set and forget, get notified,
* Added: Feature Requests #120: Scheduled backup function
* Added: Feature Requests #123: Add Ondrive backup
* Added: Feature Requests #130: WooCommerce Support on Variables Scanner
* Added: Feature Requests #137: ADD OEM Login Page
* Enhancement: Cloud backup folder structure now includes better support for multiple sites backup
* Enhancement: Schedule Scanner minor UI Improvements
* Enhancement: Save backup time of new backups made
* Enhancement: Schedule Task toggle Activate/Deactivate
* Enhancement: Improvements #121: Dashboard Links to Data
* Enhancement: Numerous other minor Enhancements and fixes
* Enhancement: Improvements #126: curb Session: Login Status
* Fixed: Schedule Scanner failed for a few users
* Fixed: Bugs #122: Dashboard popup error, on low resource servers.
* Fixed: Bugs #125: Dropbox Unlink Account Fails to Relink later
* Fixed: Bugs #129: Fix Audit my Site broken actions
* Fixed: Bugs #132: Fix CronJobs Msg: Link for “contact support team” in WP
* Fixed: Bugs #142: Virus Scanner Maximum Database connection saving error
* Fixed: Several minor tweaks and fixes

4.7.1

* Enhancement: Improve the IP Mask function in the Add IP Form
* Fixed: Some whitelisted variables are still being scanned in Basic Firewall
* Fixed: Fixed ‘PhpmailerException’ class redeclaration issue

4.7.0

* Added: Feature Requests #87: Add self unblock support
* Added: Feature Requests #90: OEM user access curb
* Added: Feature Requests #92: Ability to edit alert notification email template
* Enhancement: Improvements #96: For admin to receive emails, adding the domain in the email so the administrator knows which domain the attack is from
* Enhancement: Improvements #97: Add units on traffic map and fix Facebook like box errors
* Enhancement: Improvements #106: Improve the block page layout and design
* Enhancement: Improvements #108: Only send email out when the domains are matched in the attack
* Enhancement: Improvements #115: Log in page improvement and bug fix
* Fixed: Bugs #89: Virus Scanner Cronjob Stops
* Fixed: Bugs #93: Language codes missing in Admin email panel
* Fixed: Bugs #102: IP address not showing correctly when suite installed on Mac
* Fixed: Bugs #109: Windows server support (from Scott)
* Fixed: Bugs #110: Subscription Logout 500 Internal Server Error
* Fixed: Subscription checkout JQuery tag
* Fixed: Various other minor bug fixes and improvements

4.6.2

* Fixed: Fixed Windows server cannot add IP into the database issue – Credits to Scott Berry (www.processingpoint.com) to report this issue
* Fixed: Fixed IP cannot be added into the IP Management panel when there is a 0 on the left side of each part of the IP address

4.6.1

* Enhancement: Improve file permissions and virus scanner custom scanning directory function
* Fixed: Fix premium service page cannot login issue

4.6.0

* Added: Feature Requests #7: Dropbox Backup
* Added: Feature Requests #14: More functions in Scan Report
* Added: Feature Requests #71: Add a filter into the IP management section to filter IPs for specific type of variable
* Added: Feature Requests #84: Add directory tree map into the virus scanner
* Added: Feature Requests #86: Add a function to insert the oem customer id into the Configuration table
* Added: Feature Requests #90: OEM user access curb
* Enhancement: Added the direct access link to the IP address that is reported as spammers by the spammer detection function.
* Enhancement: Improvements #76: Add Subscription modal to the premium service
* Fixed: Bugs #45: Export IP to CSV
* Fixed: Bugs #46: Geo Data progress bar goes beyond 100%
* Fixed: Bugs #69: Foreign Language not showing properly
* Fixed: Bugs #73: Virus scanner cannot complete virus scanning
* Fixed: Bugs #88: Suite Administrator Menu Visual Bug
* Fixed: Bugs #95: Cannot add domains in Administrator Management

4.5.2

* Fixed: fixed ajax action ‘addorder’ and ‘getPaymentAddress’ not added into the ajax library for the subscription controller

4.5.1

* Minor Enhancement: improve new email notification function to increase efficiency
* Minor Enhancement: improve updater to update to 4.5.0

4.5.0

* Fixed: Bugs #15: IP management some flags are missing for some websites
* Fixed: Bugs #53: Fix variable cannot be added to suite / joomla in some websites
* Fixed: Bugs #55: In a specific website website, the variable Whitelist not working
* Fixed: Bugs #56: In a specific website, the OSE Security Suite cannot upgrade to Centrora Security Suite
* Fixed: Bugs#57: In a specific website, user cannot login premium service
* Fixed: Bugs#63: In a specific website, Virus scanner cannot complete virus scanning
* Added: Feature Requests #16: Add an email notification when the backup is completed
* Added: Feature Requests #24: Add One Click fix for file permissions functions
* Added: Feature Requests #44: Add multiple email alert receivers facilities
* Added: Feature Requests #49: Add landing page to show all features for the premium service
* Added: Feature Requests #72: Add database version to ensure smooth database updates
* Added: PDO class activation codes in the php.ini activation section for suite version
* Enhancement: UI #50: Change the one column login UI to two columns UI
* Enhancement: UI #51: Add a button to the activate my premium page to smooth premium service activation
* Fixed: Bugs #15: IP management some flags are missing for some websites
* Fixed: Bugs #53: Fix variable cannot be added to suite / joomla in some websites
* Fixed: Bugs #55: In a specific website website, the variable Whitelist not working
* Fixed: Bugs #56: In a specific website, the OSE Security Suite cannot upgrade to Centrora Security Suite
* Fixed: Bugs#57: In a specific website, user cannot login premium service
* Fixed: Bugs#63: In a specific website, Virus scanner cannot complete virus scanning

4.4.0

* Added: Backup function for database and files for the whole WordPress and Joomla website
* Added: File permission function to change the file permissions of the system
* Added: Added email for the virus scanning cronjob when the scanning is completed
* Fixed: In Windows server, the IP cannot be added into the database
* Fixed: Virus Cronjob cannot be completed in some servers

4.3.8

* Fixed: Scanning specific path not working properly on some servers

4.3.7

* Enhancement: adjusted maximum threshold function to block an IP address so it will block the IP once it exceeds the threshold instead of blocking the IP in the next time
* Added: Added single thread scanning function so the scanning can be performed on some servers with strict database connection requirements.
* Added: Backup, Clean, Delete function in scanning report
* Fixed: Scanning specific path not working properly on some servers
* Fixed: Fixed Autoloader not working when the firewall is activated globally in the php environment where local php configuration is not allowed

4.3.6

* Enhancement: Improved virus scanner
* Added: Added CURL method to download the update package
* Added: Added Backup, Clean, Backup Clean function for virus scanning report
* Added: Added Activation with Activation code function for premium services

4.3.5

* Added: Added highlight of the virus scanner report
* Enhancement: Enhance the firewall function to ignore json format request variables

4.3.4

* Enhancement: Forced display_errors to be disabled when running the Centrora Firewall for all instances
* Enhancement: MainWP Extension to support some commercial MainWP addons

4.3.3

* Enhancement: Improved MainWP Extension so it checks if the extension is enabled in the Child websites

4.3.2

* Enhancement: Changed MainWP Class loaded inside wordpress backend

4.3.1

* Enhancement: Improved virus scanner so it can scan a larger amount of files in the system
* Enhancement: Improved virus scanner for cronjob virus scanning functions
* Enhancement: Minor CSS style improvement to enhance the UI
* Added: Added MainWP Extensions Support
Fixed: Fixed the Composer class has been declared in some Joomla websites

4.3.0

* Enhancement: Improved user interface
* Added: Cron job for virus scanning (automatic daily virus scanning)

4.2.2

* Enhancement: Separate the Firewall Configuration Page and the Firewall Rules Fine-tuning page
* Enhancement: Added explanations of each ruleset in the basic firewall to let customers know more about the how Centrora Security

4.2.1

* Fixed: Custom Ban Page cannot be saved successfully on some servers.
* Added: Added version check and plugin update function

4.2.0

* Fixed: Mailer not sending email correctly when SMTP is on
* Fixed: Login panel not working when in Security Suite mode for Joomla websites
* Added: Added Custom Redirection function for users who has a custom ban page
* Fixed: Fixed Warning Errors in Anti-Spamming function
* Fixed: Fixed the email notification being sent even the Configuration Option ‘Receive Centrora Firewall / SafeBrowsing Update Email’ is set to Off

4.1.8

* Fixed: Fixed warning error reported by AlanP57: Undefined index: option in wp-content/plugins/ose-firewall/vendor/oseframework/wordpress.php on line 50

4.1.7

* Enhancement: Further Improved Anti-Spam function for registration form which blocks the spammer directly

4.1.6

* Added: Added Anti-Spam function for registration form

4.1.5

* Fixed: Fixed Configuration Window being covered by the left administrator menu in WordPress CMS – Credits to Tina Granzo (www.citybeautifuldesign.com)
* Fixed: Fixed typo error in Virus Scanner panel – Credits to Tina Granzo (www.citybeautifuldesign.com)
* Fixed: Fixed typo error in .htaccess activation codes
* Enhancement: Further Improved Alert Email

4.1.4

* Improved: Improved Alert Email
* Fixed: Fixed Virus Scanner cannot be loaded in Google Chrome in some servers

4.1.3

* Improved: Further Improve virus scanner to avoid server timeout issue for some resources limited servers

4.1.2

* Improved: Improve virus scanner to avoid server timeout issue for some resources limited servers

4.1.1

* Improved: Improve respond actions for virus scanner to handle network error
* Improved: Added restrictions on SQL user connection for Virus scanner, so it will queue until the connection is released to avoid heavy mysql server load
* Improved: Improved language tags in the virus scanner
* Improved: Improved Development mode detection function to avoid errors for some servers

4.1.0

* Added: Added rule to protect WordPress Admin Ajax file being attacked by LFI attack
* Improved: Improved Dashboard layout

4.0.9

* Improved: Improved security badge widget
* Added: Added Badge Status Checking in Audit panel

4.0.8

* Added: Added Safe Browsing Checking Information table in Audit panel
* Added: Affiliate Tracking Code Input Form in Audit Panel
* Fixed: Administrator email address not show up correctly in Firewall Configuration form.

4.0.7

* Added: Added System Pre-requisites check before framework is loaded

4.0.6

* Added: Add debug mode to avoid exception handler catch global errors

4.0.5

* Enhancement: Improve javascript for account validation function in the login panel

4.0.4

* Fixed: Fixed dashboard not Javascript function not correctly in Google Chrome version 39.0.2171.65
* Fixed: Fixed Google 2-Step Verification Configuration not showing correctly in version 4.0

4.0.3

* Enhancement: Improved scanning class to harden protection and avoid IP spoofing
* Enhancement: Improved dashboard section to avoid CSRF attack
* Fixed: Fixed error warning for WordPress website with lower version

4.0.2

* Added: Added PHP version to check ensure the PHP version (5.3.0) requirement is fulfilled.

4.0.1

* Fixed: Account action not loaded properly in My Premium Service Panel

4.0.0

* Enhancement: Completely rewrite User Interface which is fully responsive
* Enhancement: Completely rewrite framework to reduce database connection and memory usage
* Enhancement: Completely rewrite framework to enhance efficiency in detecting hacking attempts
* Enhancement: New virus scanning architect to simultaneously scan all types of viruses in the server which makes the scanning faster and consume less CPU sources

3.8.4

* Fixed: Fixed incorrect database export download link issue

3.8.3

* Fixed: Fixed database export download link returns 0 issue.
* Enhancement: Enhance the virus scanning function to ignore the parent path of scanning path

3.8.2

* Fixed: Fixed a bug caused by the conflict setting in Country blocking and Basic Firewall configuration

3.8.1

* Fixed: Fixed database table cannot be created in WordPress4.0
* Fixed: Fixed database table cannot be created (duplicate key error) when the database of the WordPress installation is shared with other WordPress installation

3.8.0

* Fixed: Fixed session error when the WordPress is integrating with Magento
* Enhancement: Improved virus scanner class to avoid multiple process being created
* Added: Added dropbox backup function in backup section

3.7.2

* Fixed: Fixed the ip2long function overflow issue for 32bit servers
* Enhancement: Improved the manage IP javascript functions

3.7.1

* Added: Added Custom Scanning Path in Virus Scanning section

3.7.0

* Added: Added Export IP function in the IP Management Section
* Enhancement: Add page size and sorting filters in the country section

3.6.6

* Enhancement: Improve database class to reduce database connections
* Enhancement: Improve backup page interface
* Enhancement: Improve Converter function to work with array variables
* Enhancement: Improve IP block function to fit with the scanning result in SQL Inject Me Firefox Addon

3.6.5

* Enhancement: Improve the IP Management Grid so the title and IPs can be copied
* Enhancement: Added Schedule Virus Scanning function for Premium service users

3.6.4

* Fixed: Fixed virus version not showing correctly issue in the Virus Scanning section

3.6.3

* Enhancement: Added advanced virus patterns in virus scanning section

3.6.2

* Enhancement: Added the page size alternation field in the IP management panel
* Enhancement: Added the function to close the SafeBrowsing window
* Enhancement: Added the data reload function for the order ascending / descending field
* Enhancement: Improved the javascript to be compatible with the https protocol
* Enhancement: Improved the variable filter function for Advanced Firewall function

3.6.1

* Enhancement: Added sorting filter and page size field in the IP Management Panel
* Enhancement: Added database object closure in the firewall scanning object to reduce redundant database connections
* Enhancement: Updated Advanced Firewall Version

3.6.0

* Fixed: Fixed the Daily Audit Report not sending out on some servers bug
* Enhancement: Added PHP Configuration Audit in Daily Audit Report

3.5.9

* Fixed: Fixed the Basic Rule title not showing correctly in the basic firewall rules section
* Enhancement: Improved the receive Centrora Firewall email function for premium service
* Enhancement: Improved the convertVariables function to convert variables when they are array
* Enhancement: Added the check Database ready function to the badge widget to avoid errors
* Enhancement: Added the PHP configuration checking in the Daily Audit Report
* Enhancement: Added PHP security enhancement function in the configuration section

3.5.8

* Fixed: Fixed the index undefined warning error in the getDisableFunctions function in Audit class

3.5.7

* Enhancement: Updated the email function to reduce duplicated emails being sent when an attack is found
* Enhancement: Updated all files to add ‘Direct access denied’ function to enhance security
* Enhancement: Extended the time difference for the safe browsing status checking
* Fixed: No sender information in the alert email when attack is detected
* Added: Added the Change All Country function into the Country Block page
* Added: Added the receive Centrora Firewall email option in the scanning configuration
* Fixed: Fixed the multiple countries status change function not working correctly in Country Block Page.
* Enhancement: Improved Scanning Configuration layout
* Added: Added PHP Configuration Auditing function to enhance overall security

3.5.6

* Fixed: Fixed configuration page not showing correctly on non-English websites
* Fixed: Fixed records cannot be deleted issues in Admin-Email Mapping section

3.5.5

* Added: Added API Configuration View in Configuration section.

3.5.4

* Added: Added option to turn on and off Daily Audit report
* Updated: Updated the firewall rules version
* Fixed: Fixed a minor warning bug in the installer for checking country database
* Fixed: Fixed a minor warning bug in the getSafeBrowsingStatus function in the Audit class
* Enhancement: Improved the virus scanning function to reduce overall memory usage
* Enhancement: Improved Configuration model to avoid warning errors in PHP strict mode
* Enhancement: Improved CountryBlock model to avoid warning errors in PHP strict mode
* Enhancement: Improved CountryBlock class to reduce duplicated download of SQL files if it has been downloaded
* Enhancement: Improved Variable function to work with both Joomla and WordPress
* Enhancement: Improved ClamD class to avoid warning errors in PHP strict mode
* Enhancement: Improved Firewall Statistics class to work with both Joomla and WordPress
* Enhancement: Improved getSafeBrowsingStatus function to avoid warning errors in PHP strict mode
* Removed: API Key in configuration section depreciated since this version.

3.5.3

* Fixed: Remove old url and Update url links in the firewall badge
* Added: Added safebrowsing checkup function in dashboard
* Updated: Updated the remote login class to allow automatic status update for premium service users
* Fixed: Fixed development mode auditing function bug

3.5.2

* Fixed: Removed WordPress version in the signature checking function in the audit class
* Fixed: Minor bug: the getConfiguration by type function has an error in the SQL query in the statistic class
* Enhancement: Added Subscription plans and enhanced checkout procedure in advanced firewall setting section

3.5.1

* Fixed: Blank Dashboard page due to table not installed
* Added: Added daily audit report to inform administrators about the status of the security status of the website.

3.5.0

* Added: Added the Get Advance Firewall Rules function into the Advance Firewall Dashboard
* Added: Added the daily automatic update of firewall rules in the advanced firewall section
* Added: Added the daily automatic update notification for firewall rules in order to notify administrators about the updates
* Fixed: Wrong help link in the scanning report page

3.4.2

* Added: Add back API field in the configuration section for some users to test the API function.

3.4.1

* Updated: Update the Local File Inclusion rule to reduce false alert

3.4.0

* Fixed: Removed views from the database that caused the database backup and restore interruption
* Enhancement: Updated database uninstallation function to clear all Centrora tables

3.3.1

* Fixed: On some servers, the virus type table interrupts the installation process
* Fixed: Token missed in the database uninstallation page.

3.3.0

* Security Enhancement: Anti-CSRF checking for all admin tasks, credits to Juan Manuel Fernández (juanma@quantika14.com)

3.2.1

* Added: Pattern and Pattern ID in Scanning Report

3.2.0

* Removed: Advanced Firewall setting panel
* Removed: Advanced Firewall checking in Dashboard Panel
* Fixed: Google Authenticator function keeps showing disabled even it is enabled in Dashboard
* Added: Country Blocking Panel and Download function
* Added: ClamAV integration into the Virus Scanning Function

3.1.3

* Fixed: IP cannot be deleted in the IP Management Panel

3.1.2

* Removed: Removed the installation of views in the database
* Fixed: Fixed the configuration cannot be saved in windows server
* Fixed: Fixed virus scanner cannot work on Windows server
* Added: Change username for the ‘admin’ account in Dashboard

3.1.1

* Enhancement: Change some wording in the dashboard to clarify the meaning of the menus
* Enhancement: Add ‘fix it’ button at the end of every warning bar.

3.1.0

* Enhancement: Enhance dashboard layout
* Enhancement: Removed unnecessary database connections
* Added: About page to show all short links to the pages in the plugin
* Enhancement: Change the remote login function to fit Centrora Panel 1.0.7

3.0.7

* Enhancement: Use the default WordPress Contact email address in the ban page instead of the default value created in the Centrora SQL file
* Removed: removed the duplicated createTable.sql file in the data folder

3.0.6

* Fixed: On some servers, the auto loader function cause blank screen.
* Fixed: On some servers, the PDO connection exceeds the maximum number of connection configured in MySQL setting. Adding datanbase connection closing codes to resolve it.

3.0.5

* Enhancement: Added the version number in the dashboard
* Enhancement: Updated the remoteLogin class to work with Centrora Panel 1.0.5
* Fixed: On some websites, the administrator's email cannot show up in the Admin-Email Mapping Panel

3.0.4

* Fixed: On some websites, the checking of Development mode causes a blank screen
* Fixed: Missing closing tag for the warning message for development checking
* Enhancement: Warning message style improved
* Enhancement: Clarified warning message for the advance firewall setting

3.0.3

* Fixed: On some websites, the administrator's email cannot show up in the Admin-Email Mapping Panel
* Fixed: Ajax class missed the ORequest Class when Centrora Panel calls the functions in the class
* Enhancement: Added a function to check if allow_url_fopen is turned on for a website
* Enhancement: Added a function to check if Development mode is turned on for the website
* Enhancement: Added a function to check if the advanced firewall setting is turned on for the website
* Enhancement: Removed duplicated ‘Advanced Firewall’ field in the scanning configuration panel

3.0.2

* Enhancement: Improved Dashboard Layout to have more user friendly navigation
* Enhancement: Improved Configuration Layout to have clearer navigation for functions like advanced firewall setting, country block and Google Authenticator
* Enhancement: Checked if the user has used other Google Authenticator plugin than Centrora Google Authenticator before loading the Google Authenticator plugin
* Enhancement: Remove the permission denied message for Country Block Page

3.0.1

* Enhancement: Removed the secret word wording from scanning configuration page
* New: Added Advance Firewall Setting function

3.0.0

* Enhancement: Improved Backend User Interface
* Enhancement: Re-designed Virus Scanning Engine, virus scanner is now 20x faster
* Enhancement: Improved Backend User Interface
* New: Added Database Backup function
* New: Central Security Management Integration with Centrora Panel
* New: Added File Upload Scanning function
* New: Added Google Authenticator (2 step authentication) function

2.2.6

* Fixed: temporarily fix the admin-email mapping not being able to fix in Google Chrome browser
* Fixed: fixed the ‘Constant OSEAPPDIR already defined’ error
* Enhancement: Enhance the YiiBase library to avoid open_basedir curb for the library autoload function

2.2.5

* Fixed: further fix for some websites the administrator lists cannot be shown in the Admin-Email Mapping section.

2.2.4

* Fixed: admin-email mapping delete function not working in some servers because the JSON encoded ID value is escaped
* Fixed: admin-email mapping add linkage function showing incorrect return message even the linkage was added successfully

2.2.3

* Fixed the admin-email mapping controller for the incorrect return messages for the Ajax message box.

2.2.2

* Fixed some websites the administrator lists cannot be shown in the Admin-Email Mapping section.

2.2.1

* Enhancement: Remove the HTML Purifier auto register function in order to solve the 500 error issue in some server.

2.2.0

* Enhancement: Added menu bar into the curb panel for easy navigation
* Enhancement: Improved firewall statistic library to reduce PHP warning errors
* Enhancement: Improved virus scanner library to reduce PHP warning errors
* Enhancement: Improved oseAjax class to support Joomla CMS
* Enhancement: Improved oseDatabase class to support Joomla CMS
* Enhancement: Improved oseEmail class to support Joomla CMS
* Enhancement: Improved oseInstaller class to support Joomla CMS
* Enhancement: Improved oseRequest class to support Joomla CMS

2.1.4

* Enhancement: Improved Germany Language Translation. Credits to Alexander Pfabel
* Enhancement: Added the debug mode option in the configuration panel to turn off error displaying function in the frontend. Credits to Wombat

2.1.3

* Enhancement: Added the function to check if the curl_exec is enabled for a hosting account, if so, the Stop Forum Spam function will be disabled.
* Enhancement: Improve the backend css file to adjust the font-size to match default wordpress font-size. Credits to Alexander Pfabel
* Enhancement: Improve the badge seal layout and background images

2.1.2

* Enhancement: Added Germany Support – credits to: German translation by Alexander Pfabel (http://alexander.pfabel.de)
* Fixed no data issue in Admin Email Mapping config page, Credits to shadowood, and itpixie
* Enhancement: make the Admin Email Mapping Editing window closable

2.1.1

* Add back i18n multiple language solution library, some environment requires this. Credits to joedeagnon

2.1.0

* Significantly reduce package size
* Fixed Class ‘CHtmlPurifier’ not found error during database creation section. Credits to mikeotgaar
* Fixed wrong warning message shown in Variables management. Credits to shadowood, and kamill
* Fixed Virus Scanner Panel: no progression bar during scan. Credits to shadowood
* Fixed Virus Scanner Panel: no progression bar during scan. Credits to shadowood
* Fixed incorrect format for option ‘File Extensions’ in the virus scan config page. Credits to shadowood
* Fixed incorrect sizing for scan file size box. Credits to shadowood
* Enhancement: remove GeoIP database tables requirements, significantly reducing Database size. . Credits to shadowood

2.0.2

* Remove Secret Word Descriptions
* Fixed non-English website not able to load javascript language files issues

2.0.1

* Fixed Badge update issue
* Fixed Virus database update issue
* Fixed Database keeps display not ready issue

2.0.0

* Improved front-end protect seal showing function
* Rewrite the whole plugin to implement the MVC structure

1.6.4

* Improved front-end protect seal showing function
* Improved front-end protect seal CSS style

1.6.3

* Fixed the log table not created properly issues on some servers

1.6.2

* Fixed a typo in the security seal

1.6.1

* Updated Chinese and Germany languages, credits to Mr Alexander Pfabel
* Fixed the Class ‘osewpScanEngine’ not found issue for some servers

1.6.0

* Added Stop Forum Spam Anti-spamming checking, keep your blog spam free
* Added Security Protection Badge, shows the confidence of your website security to your clients
* Added the logs of virus scanning to show the scanning records in the security protection badge

1.5.4

* Removed duplicated menus as suggested by Lime Canvas (https://wordpress.org/support/profile/limecanvas)
* Fixed the issue where OSE Firewall Settings links are appended to all plugins links section (credits to Lime Canvas https://wordpress.org/support/profile/limecanvas)
* Fixed the wpdb undefined issue when initializing file list into the database

1.5.3

* Updated the codes to make it work with multiple websites (credits to scottnath, https://wordpress.org/support/profile/scottnath)
* Improved function to check admin accounts
* Fixed PHP warning errors for undefined OSE Firewall setting variables

1.5.2

* Updated Chinese and Germany languages, credits to Mr Alexander Pfabel

1.5.1

* Fixed back-end admin menu causing warning message issues (reported by mike http://www.graphicline.co.za/ and Alan https://wordpress.org/support/profile/alanpae, AlanP57 https://wordpress.org/support/profile/alanp57)
* Fixed language file loading error issue (credits to scottnath, https://wordpress.org/support/profile/scottnath)
* Fixed redirection function error issue reported by numzi https://wordpress.org/support/profile/nunzi
* Avoid scanning back-end blog post action to avoid false alerts with javascript codes inserted in to blog posts (thanks for the report by Alexander https://wordpress.org/support/profile/herzwacht and

1.5.0

* Added four protection modes: OSE Firewall only, OSE Security Suite only, OSE Firewall plus OSE Security Suite and Development mode (protection temporarily turned off)
* Added a server IP field to avoid false alerts due to empty user agent
* Fixed the field ‘Detect Directory Traversal’ not being saved properly issue
* Added custom banning message field and custom banning message function
* Enhance OSE Banning page appearance
* Enhance Javascript injection detection pattern to avoid false alerts
* Added OSE Virus / Malicious codes scanning function

1.0.2

* Added Germany Translation language
* Added the maximum tolerance parameter, so the attacker will be blocked automatically after X times of attack

1.0.1

* Added French Translation language

1.0.0

* Initial release