
CloudFiles Backup/Restore Scripts
=================================

Python scripts to backup and restore to/from Rackspace CloudFiles.

Written because I need to sometimes quickly back up and restore things
offsite without thinking.

Before using update the accounts hash to include username and api key.
In theory, you could add additional hashes to the list to backup to two
seperate cloud accounts at the same time in different regions (though
this has not been tested yet..)

To backup:
==========

backup_to_cloud <filename>

or 

backup_to_cloud <directory> 

Note: If the file already exists on cloudfiles, it is overwritten.


To restore: 
===========

TBD.
