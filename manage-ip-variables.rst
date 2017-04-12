Manage IPs and Variables
*************************

1. After the configuration is done, we can now test the protection to make sure it’s working on the site. Please use the URL below for testing:
http://your_site_URL/index.php?a=%27union

You should get the block page if you didn’t set the Silent Mode ON in the Advanced Configuration (which is only available for premium members). The block message can be customized in the SEO Configuration.

<a href="http://googledrive.com/host/0B4Hl9YHknTZ4aGpiTXFHOTVYdjA/ipv_1.jpg" target="_blank"><img class="wp-image-2830 alignnone" src="http://googledrive.com/host/0B4Hl9YHknTZ4aGpiTXFHOTVYdjA/ipv_1.jpg" alt="001" width="760" height="300" /></a>

<em>For premium users, We strongly recommend you to turn on the Silent Mode after the testing.</em>

2. After the testing finishes, the IP record will be logged in the menu <strong>Protect → IP Control</strong>. An IP record can have 3 states, Whitelisted, Blacklisted, and Monitored. “Whitelisted” (marked as a green check) means the IP will not be scanned by the Firewall core engine; “Blacklisted” (marked as a red stop symbol) means the IP will be thoroughly blocked from the site and receive the block message; and “Monitored” (marked as a yellow eye) means the IP is only logged in IP Management for the admin attention and the IP will still have access to the site.

<a href="http://googledrive.com/host/0B4Hl9YHknTZ4aGpiTXFHOTVYdjA/ipv_2.png" target="_blank"><img class="wp-image-2830 alignnone" src="http://googledrive.com/host/0B4Hl9YHknTZ4aGpiTXFHOTVYdjA/ipv_2.png" alt="001" width="760" height="300" /></a>

You can manage IPs with the functional buttons.
<ul>
 	<li><strong>Add IP:</strong> It can add new IP rule to define new IP or IP range whitelist and blacklist. In the IP RuleTitle field, you can input anything which can remind you of the reason for adding the rule.</li>
</ul>
<a href="http://googledrive.com/host/0B4Hl9YHknTZ4aGpiTXFHOTVYdjA/ipv_3.png" target="_blank"><img class="wp-image-2830 alignnone" src="http://googledrive.com/host/0B4Hl9YHknTZ4aGpiTXFHOTVYdjA/ipv_3.png" alt="001" width="760" height="300" /></a>
<ul>
 	<li><strong>Blacklist IPs/Whitelist IPs/Monitor IPs:</strong> ou can use these buttons to switch between different IP states for a chosen IP.</li>
 	<li><strong>Delete Items/Clear All Items:</strong> To delete some or all existing IP rules in the IP Management.</li>
 	<li><strong>Update Host:</strong> To keep the host information of the IP up to date.</li>
 	<li><strong>Import/Export IP from/to CSV:</strong> The tool for importing or exporting IP rules.</li>
</ul>
3. Sometimes, you may need to check record details to find the reason for being logged in IP Control to judge if it’s a real hacking attack or a false alert, especially when you just start using the Firewall system. Based on the detailed information, you can whitelist the false alerted variables to make the system fit your site’s functions and make it more stable. To do this, please click on Action following an IP to review the details first.

<a href="http://googledrive.com/host/0B4Hl9YHknTZ4aGpiTXFHOTVYdjA/ipv_4.png" target="_blank"><img class="wp-image-2830 alignnone" src="http://googledrive.com/host/0B4Hl9YHknTZ4aGpiTXFHOTVYdjA/ipv_4.png" alt="001" width="760" height="300" /></a>

<a href="http://googledrive.com/host/0B4Hl9YHknTZ4aGpiTXFHOTVYdjA/ipv_5.png" target="_blank"><img class="wp-image-2830 alignnone" src="http://googledrive.com/host/0B4Hl9YHknTZ4aGpiTXFHOTVYdjA/ipv_5.png" alt="001" width="760" height="300" /></a>

As screenshot shows, you can find two important values–Detected Variable and Detected Content. From the example of test with index.php?a=%27union, the variable is “get.a” and the blocked content is “union”. You can know it’s a hacking attack from the blocked content. If the content is some legitimate text, for example you submit some text in the article which contains a sensitive word falsely alerted, you need to set the IP as “Monitored” and also whitelist the Variable in Variables Management to avoid it happening again in the future.

4. When you believe an IP is falsely logged and the variable is frequently falsely alerted , you can whitelist the variable in Variables Management. Go to the menu<strong> Protect → Variables List</strong>. Let’s still take the above test as example and assume it’s a false alert. You can find all existing logged variables there and locate the one which we are going to whitelist based on the variable value “a”. Choose the variable and use the “Ignore the Variable” button to whitelist it.

<a href="http://googledrive.com/host/0B4Hl9YHknTZ4aGpiTXFHOTVYdjA/ipv_6.png" target="_blank"><img class="wp-image-2830 alignnone" src="http://googledrive.com/host/0B4Hl9YHknTZ4aGpiTXFHOTVYdjA/ipv_6.png" alt="001" width="760" height="300" /></a>

In the Variables Management section, each variable also has 3 possible states to choose from.
<ul>
 	<li><strong>Scan the Variable:</strong> It means the Firewall engine will actively scan for the variable’s content and block the IP if it violates the Firewall rules.</li>
 	<li><strong>Filter the Variable:</strong> It means the Firewall engine will still scan the variable’s content and log any suspicions, but it will not block the IP. This it for cases in which you are not sure whether the variable needs to be whitelisted and want to collect more information.</li>
 	<li><strong>Ignore the Variable:</strong> This means the variable is thoroughly whitelisted and the variable’s content will not be scan any more.</li>
</ul>
5. <strong>Load default whitelist variables.</strong> After installing the Firewall system, we strongly recommend you to load the default whitelist variables for Joomla!, and also load the default whitelist variables for JomSocial if you have it installed. This will reduce the number of false blocks for normal Joomla! sites and JomSocial users.
