Dynamic Scanner and Virus Cleaning
**********************************

<h3>Virus Scanner - Dynamic Scan</h3>
Centrora Security system integrates a Virus Scanner - Online Antivirus tool for scanning and cleaning the website which has been compromised. Currently, the scanner is available for Free users, however, the detailed scan result and cleaning operations are only available for Premium Subscribers. Also, please note that the scanner only scans the file system but not the database.

Please refer to the video for How to do a quick dynamic scan for the website.
<iframe width="760" height="500" src="https://www.youtube.com/embed/v3EmRsipAWM" frameborder="0" allowfullscreen="allowfullscreen"></iframe>

Also, watch the video for how to review the scan result and clean the files.
<iframe width="760" height="500" src="https://www.youtube.com/embed/HyL7mMv3tk4" frameborder="0" allowfullscreen="allowfullscreen"></iframe>

Or, please follow the below steps to do a full website scan.

Let's start a scan now. please go to the menu <strong>Search for Malware</strong> → <strong>Dynamic Scanner</strong>. It will show the main operation panel of the scanner.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/100_Dynamic_Scanner.jpg" alt="Dynamic Scanner" width="900" />

<strong>1.</strong> First, please configure file extensions, maximum file size, etc for the scan in the button "<strong>Config Setup</strong>". The unit for file size is MB. <strong>Maximum Database Connection</strong> is an advanced parameter. If you know the DB connection limit on your server, please set the parameter accordingly; and please set it as 50 or 100 if you have no idea about it. For the Max Execution Time, you can set it as 300.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/101_Dynamic_Scanner_Config.jpg" alt="Config Config Setup" width="900" />
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/102_Dynamic_Scanner_Configuration.jpg" alt="Configuration" width="900" />

<strong>2.</strong> <strong>Select Scan Types</strong> to choose what types of virus you are going to scan. Generally, if you have no idea about it, please just choose <strong>Deep Scan</strong> to do a full scan.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/103_Dynamic_Scanner_Scan_Types.jpg" alt="Select Scan Types" width="900" />

<strong>3.</strong> Now we can start a scan. By simply click the <strong>START</strong> button, it will do a full website scan.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/104_Dynamic_Scanner_Start_a_Scan.jpg" alt="Start a Scan" width="900" />

If you just want to scan a specific target or some folder outside of the current website root, you can use <strong>Scan Specific Folder</strong> to choose the folder or define the path to scan. (1) Click the small folder icon to extend the sub-folders/files tree under the folder. (2) Please note that if you enter the path value manually, it requires the absolute path. (3) Click the button to start the scan.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/105_Dynamic_Scanner_Scan_Specific_Folder.jpg" alt="Scan Specific Folder" width="900" />

<strong>4.</strong> During the scan, the main panel will show the progress and also the status of the server memory and CPU usage. During the scan, you can use <strong>STOP</strong> button to cease the process and then use "Continue" button to re-start it from the previous stop point. After the scan completes, it will give a brief scan result.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/106_Dynamic_Scanner_Scan_Complete.jpg" alt="Scan Complete" width="900" />

<strong>5.</strong> Now we can view the scan result in the menu <strong>Search for Malware</strong> → <strong>Scan Result</strong>. It is highly recommended that before you clean or quarantine any of the reported files, double-check whether they are truly infected with the virus or a false positive. It's because that Virus Scanner might occasionally trigger false alerts on some legitimate files. Clicking on View and checking the file codes manually can reduce the possibility of falsely deleting any system core files.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/107_Dynamic_Scanner_Scan_Result.jpg" alt="Scan Result" width="900" />

After clicking the View button, the Scanner will pop out a window to show the file codes and also highlight the codes that are recognised as malware.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/108_Dynamic_Scanner_View_Codes.jpg" alt="View Codes" width="900" />

<strong>6.</strong> We have some optional Actions to deal with the files after reviewing the codes.
<ul>
 	<li><strong>A.</strong> We can choose to clean the highlighted suspicious codes if the codes are just injected into a functional file. Use the "Clean" button on the code viewing window or after selecting the file in the scan result panel.</li>
 	<li><strong>B.</strong> Alternatively, if you find that all the codes in the file are malware codes, please "Quarantine" the file entirely as the file could be uploaded by the hacker.</li>
 	<li><strong>C.</strong> If you think it's a false alert, you can "Mark as Clean" to whitelist it.</li>
 	<li><strong>D.</strong> Also, if you find the website doesn't run correctly after you clean or quarantine some file, you can use "Restore" button to restore it to the original copy before the operation.</li>
 	<li><strong>E.</strong> If you find that the Scanner only marks the key patterns of the virus, rather than highlighting all the codes infected, the file needs to be cleaned manually. You need to do this via an FTP or the File Manager in your Host Control Panel.</li>
</ul>
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/109_Dynamic_Scanner_Action.jpg" alt="Actions" width="900" />

<strong>7.</strong> After checking all files, you might do a scan again to verify if the website is clean. Before that, you can export the current scan/cleaning logs to a .csv file for the future reference. Simply click Export to CSV button and save the file to your PC.
<img class="alignnone" src="https://cdn.protect-website.co/centrora_web/images/Tutorials/110_Dynamic_Scanner_Export_to_CSV.jpg" alt="Export to CSV" width="900" />

Despite our best effort to keep updating the Scanner (online antivirus), it might still be unable to recognise some specific infections. In some case, some virus evolves, or the hacker alters the way they encode the virus codes. Therefore, if you believe the Scanner cannot detect all the virus files on your site, or the site still encounters problems after you clean it, please don’t hesitate to contact our Support Centre. We will arrange developers to do the check for you.
