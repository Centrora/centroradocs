Centrora Security Basic Firewall Rules Explanation
****************************************************************

* Enable Stop Forum Spam Scanning

This will check if the IP address being scanned or the email address being scanned has been marked as spammers from the `Stop Forum Spam <http://stopforumspam.com/>`_ website.

* Block Blacklisted Methods (Trace / Delete / Track)

Every time a client attempts to connect to your server, it sends a message indicating the type of connection it wishes to make. There are many different types of request methods recognized by Apache. The two most common methods are ``GET`` and ``POST`` requests, which are required for “getting” and “posting” data to and from the server. In most cases, these are the only request methods required to operate a dynamic website. Allowing more request methods than are necessary increases your site’s vulnerability. Here we are blocking delete and head because they are unnecessary, and also blocking trace and track because they violate the same-origin rules for clients. (Reference: Perishable Press)

* Checks Malicious User Agent

Blocking hundreds of the worst bots can ensure open-access for normal traffic, major search engines (Google, Bing, et al), good browsers (Chrome, Firefox, Opera, et al), and everyone else. Blocking malicious user agent can help you avoid traffics that are known to be associated with malicious activity

* Checks Basic DoS Attacks

This helps prevent your website against the HTTP Flood Attacks at the web application level. Massive crawling / scanning tools, HTTP Flood tools can be detected and blocked if it exceeds the defined thresholds / number of visits to your website in a specific time.

* Checks Basic Remote File Inclusion

Remote File Inclusion (RFI) is a type of vulnerability most often found on websites. It allows an attacker to include a remote file, usually through a script on the web server. The vulnerability occurs due to the use of user-supplied input without proper validation.

* Checks Basic Direct File Inclusion

Direct File Inclusion / Local File Inclusion (LFI) is similar to a Remote File Inclusion vulnerability except instead of including remote files, only local files i.e. files on the current server can be included. The vulnerability is also due to the use of user-supplied input without proper validation. (Reference: WikiPedia)

* Checks Basic Javascript Injection

JavaScript injection is a nifty little technique that allows you to alter a sites contents without actually leaving the site. This can be very useful when say, you need to spoof the server by editing some form options. This includes I. Injection Basics, II. Cookie Editing and III. Form Editing

* Checks Basic Database SQL Injection

SQL injection is a technique where malicious users can inject SQL commands into an SQL statement, via web page input. Injected SQL commands can alter SQL statement and compromise the security of a web application.

* Detect Directory Traversal

A directory traversal (or path traversal) consists in exploiting insufficient security validation / sanitization of user-supplied input file names, so that characters representing “traverse to parent directory” are passed through to the file APIs. (Reference: WikiPedia)

* Block Queries longer than 255 characters

Queries that are more than 255 characters long can use a lot of resources and slow your site down for legitimate users.  Usually queries longer than 255 characters have “eval” or “base64″ methods in it. This is very likely that the codes are looking for a way to inject script on your site that could create a backdoor, launch spam or some other malicious activity.