
CloudFiles Backup/Restore Scripts
=================================

NB: You probably want to be using the swift cli and not this.
    This is me messing around with pyrax.

Python scripts to backup and restore to/from Rackspace CloudFiles.

Written because I need to sometimes quickly back up and restore things
offsite without thinking.

Before using update the accounts hash to include username and api key.
In theory, you could add additional hashes to the list to backup to two
seperate cloud accounts at the same time in different regions (though
this has not been tested yet..)

Requires you to install the pyrax python module:

eg. pip install pyrax

To backup:
==========

backup-to-cloud filename

or 

backup-to-cloud directory 

Note: If the file already exists on cloudfiles, it is overwritten.


To restore: 
===========
restore-from-cloud LIST - list objects.
restore-from-cloud GET - download file to current directory

To Do:
======
- Need to add recursive restore of directory
