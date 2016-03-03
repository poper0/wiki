Tupac is a 2RU Supermicro server. The OS runs off two 64G SATA DOMs plugged directly into the motherboard, configured with a 500M /boot and a 63G / partition, each mdraided.

It has two 1TB disks configured as a mirror ZFS zvolume which appears on /data.

The machine has two Gigabit Ethernet NICs and a 10GB fiber NIC. In addition, it has an AudioScience Livewire ASI card.

One ethernet jack will be connected to the Tufts LAN, and the other connected to the internal network. Once the fileserver is migrated to Ballou, the fileserver will be connected via a 10GB GBIC patch cable to ensure speedy data transfer.

It has redundant hot swap power supplies, and it is also wired for the full 8 disks. Each of the 3.5 bays has been converted to support 2.5 inch drives with associated mounting hardware (this was done to get a cost-effective server with 4 PCIe slots, as opposed to getting a 1RU box.

The machine will not have a WAN IP (so will be accessible only through the firewall through any public server or the NAT router).

See the reference section on creating guests on the machine.

Guests

-   nick-test
-   windows10
-   windows7
-   webstream (windows 7)
-   webhost (Ubuntu - WAN)
-   database
-   email
-   Rivendell
-   Rivendell-test
-   scriptbox - used to handle routine tasks, scripts, anything remotely bash-y or hack-y, for example automatically propogating SSH keys between all other hosts as one host is updated

*No headers*
