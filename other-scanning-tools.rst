Other Scanning Tools
*********************

Besides the core Dynamic Scanner, Centrora Security system also integrates some other scan tool which can assist us to thoroughly clean the website and to confirm if the website has been fixed.

Core Directories Scanner
--------------------------

Core Directories Scanner will scan the website to compare the core system files with the original official package. Just click ``Start Scanning`` inthe menu ``Search for Malware --> Core Directories Scanner`` to do the scan. After a scan, it will report the files which are modified, removed, and suspicious compared to the original version. Take a Joomla! site as an example,

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/120_Core_Directories_Scan.jpg

.. note:: The result is just for the reference. It doesn't mean that the files listed in the result are the malware files. It's because site may have 3rd party extensions and libraries installed. So please review the files briefly to have more information. Or please `contact us <https://www.centrora.com/support>`_ for help.

Modified File Scanner
-----------------------

Sometimes, the `Dynamic Scanner <dynamic-scanner>`_ cannot finds all virus files on the sites, for example:

1. The hacker uploads the hacking files in a package and not all files there contains the virus patterns;
2. The files are encoded in a special way to hide from the scanner.

In this case, the Modified File Scanner may help which can show the files modified within a time range which we can define. For example, if we think the site was hacked on date X or we find some suspicious files with the date X, we can use Modified File Scanner to find out all files changed around date X, say (X-3, X+3). Then we can get all files which could be involved in the hacking.

Go to the menu ``Search for Malware --> Modified File Scanner``, define the date range and the scan path. Then ``Start scanning``.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/121_Modified_File_Scanner.jpg

MD5 Hash Scanner
-----------------

MD5 Hash Scanner will scan the file MD5 Hash of the core system files to report the suspicions. Please update MD5 Hash database before the scan.

.. image:: https://cdn.protect-website.co/centrora_web/images/Tutorials/122_MD5_Hash_Scanner.jpg
