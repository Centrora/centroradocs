About Centrora Git backup
********************************************

Git is a popular modern version control system.

You can think Git as a small software which constantly monitors for the changes of the file system. Unlike the traditional backup method, which will pack all the files into an archive file, Git will only keep track of changed files. The problem with the traditional backup method is that the regular backups will keep consuming the serve space. Especially, when the website is huge it becomes a big burden for the server. Consider a website is 10 GB ,and also we make the daily backup and keep them for 5 days. The server needs to keep 5 10GB backup packs for the 5 consecutive days, which is a big waste. While Git only keeps track of file changes and thus it consumes very little space between 2 different backups.

Let's show it in the chart with an example. Say there is a website which is 10GB originally. Moreover, on average, there is 100MB new data/file added to the website and we want to keep 5 daily backups.

+------+------+------+------+------+
| Day |	Site Size | New Data on the site | New Backup Size with Traditional Method |	New Backup Size with Git Method |
+======+======+======+======+======+
| 0 | 10 GB |  | 10 GB | 10 GB |
2 	105 	+105 	+5
3 	110 	+110 	+5
4 	115 	+115 	+5
5 	120 	+120 	+5
Accumulation 		+550 	+120



Note: 
If your website has too many media files it is recommended that you store them in different location than your website directory. 
For E.g.: if the website is located in: /home/abcwebsite/public_html 
the git backup will backup and keep history of all the files located in the folder: /home/abcwebsite/public_html  
if you have media files you can store them in the location : /home/abcwebsite/mediafiles
One of the drawbacks of using Git is it does not handle media files well as it keeps track of each and every line. so, when it tries to manage the version of the media files it has to store a lot of information about the media files and thus the Git folder (where git version history is stored ), may swell up and consume too much if space. If you have a low amount of media files then you can keep the same folder structure or store the media files at the default folder locations.