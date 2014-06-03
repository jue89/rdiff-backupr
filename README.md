rdiff-backupr
=============

What the heck?
--------------

**rdiff-backupr** helps you keeping your backups nicely organised configured just by some easy readable text files. As you might expected, it uses *rdiff-backup* in the background. And yes, its name is kind of silly. But hey - it's just a quick and dirty hacked CLI-PHP-Script. In the end its working for all my use cases.

This script has been tested with Debian and Ubuntu.


Requirements
------------

- rdiff-backup
- php5-cli
- cron or something like that


Install
-------

- Clone this repository.
- Make sure *backup* is executable.
- Create a directory where you would like to keep you backups.
- Copy *rdiff-backupr.conf.sample* to your home directory and name it *.rdiff-backupr.conf*
- Edit *~/.rdiff-backupr.conf*
- Optional: Create a cron job that calls *backup* regularly. (Further details in section Usage.) Don't forget to specify a eMail address for delivering logging informations. **I highly recommend to check these logs!**


Configure a backup
------------------

- Go to your specified directory for your backups.
- Create a directory with a witty name. Boring people may chose the hostname of the source machine.
- Copy *backup.conf.sample* to the brand new directory and name it *backup.conf*
- Edit *backup.conf*


Usage
-----

$ backup [{config}]

- config: Optional. Path to a configuration file.
