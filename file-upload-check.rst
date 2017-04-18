File Upload Validation
***********************

Centrora Security integrates a File Upload Validation function to stop the malware files upload from the website forms.

.. warning:: Please note that the FILEINFO module needs to be installed properly on the server to have the function working correctly. More information about FILEINFO can ne found at: http://php.net/manual/en/ref.fileinfo.php

If there is no FILEINFO on the server or if you have any trouble uploading files even with the extensions whitelisted, please consult the Host to make sure if it’s been installed on the server.

First, the feature will only allow the files to be uploaded with extensions that you mark as Whitelist. Also, it will scan the extension of the uploaded files to check the consistency of its extension and the real type. This will block the files with hacking codes embedded.
Please configure the settings in menu Protect → Upload Control.

001

The extensions with a green check are allowed to make uploads while those with a red cross are not. You can also add more extensions if the default list doesn’t include your file type.

In ‘File Uploading Log’, you can check all the files uploaded with the function enabled. When the site has any anomaly, you might need to investigate all the changes made to the site within a certain period of time, and this can be helped by the log.