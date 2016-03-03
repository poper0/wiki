We utilize two large RAID6 arrays to host dual, parallel copies of our primary data store. For performance reasons, the 'primary'  data store for a given top level directory depends on the directory in questions. The table below shows which server is the primary for each directory. The server on the left of the backup arrow (which should equal the SMB server) is the primary server.

 As of of January 2013, around 12.1TB of 17.5TB (70%) of the disk space is used.

Rationale
---------

We will attempt to keep each storage array a perfect mirror of the other (within a given backup interval) to simplify backup and failover operations. Automatic backup jobs will be put in place after the [Fall 2011 storage upgrade](https://wiki.wmfo.org/Operations/Historical/Fall_2011_Data_Server_HD_Upgrade "Fall 2011 Data Server HD Upgrade") to automatically backup each directory from it's primary to secondary server as reflected below.

 

Under normal operation, please only access files for a given data directory via the primary server for that directory. Some backup jobs may only perform primary-\>secondary backups, so changes made directly to the secondary server for a given directory are liable to be out of date or overwritten. Under certain conditions (server failure, etc), it may be necessary to access the secondary store directly, but please consult the [Operations Director](https://wiki.wmfo.org/Executive_Board/Operations_Dept. "Operations Dept.") before doing this.

Data Drive Directory Structure
------------------------------

---Directory---   ---------Description---------   --Hierarchy--   -BUType-   ---SMBShare---       

VirtualMachines - VM Datastores                 - Smooth-\>Super - Echo     - Virt...-Smooth

PublicFiles     - [files.wmfo.org](http://files.wmfo.org/ "http://files.wmfo.org/") Public Files - Smooth-\>Super - Echo     - Public-Smooth

FTP             - WMFO Main FTP Files           - Smooth-\>Super - Echo     - FTP-Smooth

EAS             - EAS FTP Files                 - Smooth-\>Super - Echo     - EAS-Smooth

Rivendell       - Rivendell Music and Audio     - Super-\>Smooth - Contrib. - Rivendell-Super

tobeImported    - Ripped Music and Audio        - Super-\>Smooth - Echo     - tobe...-Super

Archive         - WMFO Archived Audio and Media - Super-\>Smooth - Contrib. - Archive-Super

Backup          - WMFO Backup Jobs Data Store   - Super-\>Smooth - Contrib. - Backup-Super

Data            - Misc Data Store               - Super-\>Smooth - Synch.   - Data-Super

1.  1. [Rationale](#Rationale)
2.  2. [Data Drive Directory Structure](#Data_Drive.C2.A0Directory.C2.A0Structure)

