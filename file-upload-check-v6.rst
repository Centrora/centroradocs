File Upload Validation
***********************

Centrora Security integrates a File Upload Validation function to stop the malware files upload from the website forms.

.. note:: Please note that the *FILEINFO* module needs to be installed properly on the server to have the function working correctly. More information about *FILEINFO* can ne found at: http://php.net/manual/en/ref.fileinfo.php

Switch On/Off File Upload Validation
-----------------------------------------

If there is no *FILEINFO* on the server or if you have any trouble uploading files even with the extensions whitelisted, please disable the function in the menu ``Firewall Setting --> Firewall Rules Fine-tunings --> Basic Firewall Rules``, page 2, **File Upload Validation** by clicking the Status icon to make it inactive.

.. image:: https://cdn.centrora.com.au/images/Tutorials/315_File_Upload_Validation.jpg

Configuration
--------------------------

First, the feature will only allow the files to be uploaded with extensions that you mark as **Allowed**. Also, it will scan the extension of the uploaded files to check the consistency of its extension and the real type. This will block the files with hacking codes embedded.
Please configure the settings in the menu ""Logs --> File Uploading Logs --> FIle Extension List``. The extensions with a green check are allowed to make uploads while those with a red cross are not. You can also add more extensions if the default list doesn't include your file type.

.. image:: https://cdn.centrora.com.au/images/Tutorials/316_File_Extension_List.jpg

In the tab of the same menu ``File Uploading Log``, you can check all the files uploaded/blocked with the function enabled. When the site has any anomaly, you might need to investigate all the changes made to the site within a certain period of time, and this can be helped by the log.