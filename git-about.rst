About Centrora Git backup
********************************************

Choosing a proper backup way is always an important topic for website administrators. It helps keep the site data safe and guarantees that we have the latest working version under any circumstances. Super fast, efficient, and reliable, the technology with Git, which brings us many miracles, strives to provide the best solution for the object.

 **Why choose Git?**


Git is a popular modern version control system. You can think Git as a small software which constantly monitors for the changes of the file system. Unlike the traditional backup method, which will pack all the files into an archive file, Git will only keep track of changed files. Compared to traditional backup methods, the technology with Git has 4 significant advantages.

1. Efficient in resource consumption
--------------------------------------------

Git only tracks the changes. So not like the traditional backup method, it will not keep the full website files and data upon each backup. Only changes will be committed to the last backup package and it records the complete history. So after the first time initialization, it takes much less space and saves a lot of time in a new backup.
To make a comparison, let’s take an example of a website with 100MB originally and assume the size increases by 5MB every day due to new contents, user data, and logs and we make a full backup for the site every day. So the site size will be 105MB on the 2nd day, 110MB on the 3rd day, 115MB on the 4th day,and so on. At the beginning, the backup package size is 100MB, the same for the traditional and Git methods.

+------+------+------+------+
| Day |	Site Size | New Added Backup Size with Traditional Method |	New Added Backup Size with Git Method |
+======+======+======+======+
|  1 | 100 MB | 100 MB | 100 MB |
+------+------+------+------+
|  2 | 105 MB | 105 MB |   5 MB |
+------+------+------+------+
|  3 | 110 MB | 110 MB |   5 MB |
+------+------+------+------+
|  4 | 115 MB | 115 MB |   5 MB |
+------+------+------+------+
|  5 | 120 MB | 120 MB |   5 MB |
+------+------+------+------+
|  6 | 125 MB | 125 MB |   5 MB |
+------+------+------+------+
|  7 | 130 MB | 130 MB |   5 MB |
+------+------+------+------+
|  8 | 135 MB | 135 MB |   5 MB |
+------+------+------+------+
|  9 | 140 MB | 140 MB |   5 MB |
+------+------+------+------+
| 10 | 145 MB | 145 MB |   5 MB |
+------+------+------+------+
| Accumulation |  | 1225 MB |   145 MB |
+------+------+------+------+

However, we can observe the dramatic difference just after 10 days. With the traditional method, it keeps the full daily backups. So if we save the backup packs for all the 10 days, the total space on the server reaches 1225 MB; while the Git method only consumes 145MB as it only commits the change of 5MB every day, at the same time, the backup time being largely shortened as well.

2. Super fast in rollback
With the traditional method, if our website gets hacked, we must do a full restoration. That means, we need to carefully go through the steps including, removing all the current files, uploading or extracting the files from a previous version to the server, removing the database, and restoring or importing the data from a previous backup too. Generally, it will take about 30 minutes and lots of operations.
With the Git method, just one click can resolve all the issues and it could just take less than 30 seconds because it only rollback the changed contents based on the previous version.

3. Easy to track the differences
Sometimes, we need to compare the files between different versions for development or security purposes. With the old way, it’s a big trouble especially when the site has a large number of files, because it needs us to build a mirror, restore all files of both versions,  compare the files with the MD5 Hash and even manually review the codes.
With the Git functions, it will be as easy as pie. Git is designed to have a complete history and full version tracking abilities. With a few operations, we can get a full list of changed files and also the detailed changed codes of each file.

4. Unlimited space when uploading the backup to Cloud
Cloud backup is a popular solution as we can easily bring the backup with we at any place at any time as long as there is an internet connection. Nowadays, all major Cloud services provide quite a large storage space and we may get more by paying extra for the service. However, it’s still limited. The consideration of space will more or less restricts the freedom of keeping the backup in a long term.
This is not a problem at all for Git solution. With Bitbucket free service, we can create unlimited repositories, Git work directories, and each repository offers 2GB space. It becomes so easy to keep the full history for a website as long as we want.

 The problem with the traditional backup method is that the regular backups will keep consuming the serve space. Especially, when the website is huge it becomes a big burden for the server. Consider a website is 10 GB ,and also we make the daily backup and keep them for 5 days. The server needs to keep 5 10GB backup packs for the 5 consecutive days, which is a big waste. While Git only keeps track of file changes and thus it consumes very little space between 2 different backups.

Let's show it in the chart with an example. Say there is a website which is 10GB originally. Moreover, on average, there is 100MB new data/file added to the website and we want to keep 5 daily backups.





Note: 
If your website has too many media files it is recommended that you store them in different location than your website directory. 
For E.g.: if the website is located in: /home/abcwebsite/public_html 
the git backup will backup and keep history of all the files located in the folder: /home/abcwebsite/public_html  
if you have media files you can store them in the location : /home/abcwebsite/mediafiles
One of the drawbacks of using Git is it does not handle media files well as it keeps track of each and every line. so, when it tries to manage the version of the media files it has to store a lot of information about the media files and thus the Git folder (where git version history is stored ), may swell up and consume too much if space. If you have a low amount of media files then you can keep the same folder structure or store the media files at the default folder locations.