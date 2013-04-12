kwikback
========

A series of backup scripts for my servers to move databases and site files
to VPN backup locations and quickly tie everything up into a nice package.

This custom backup script dumps all data from MySQL, backs up the site
files directory in /var/www and backs up the Apache configuration files. 

To install-- add fullbackup, mysqlbackup, and sitefilesbackup to:
    /usr/local/bin/ 
If you add it to your path, please ensure that the variables in fullbackup
are appropriately modified to handle the path of the new files. 

In fullbackup ensure that the following strings are set:
    REMOTE_DIR
    REMOTE_PORT 
So that you can scp the backup to a remote location. 

Also ensure that the directory BAK_DIR is set in your USER_DIR
