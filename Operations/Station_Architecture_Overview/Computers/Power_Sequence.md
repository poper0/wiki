You may also want to take this opportunity to run updates on all linux machines as this gives you a chance to get new kernels installed before the reboot. Samba may also be updated which normally kills Rivendell audio.

Full Power Down Sequence:

1. Grab a flashlight (optional)
2. Transmitter - power off using web interface http://transmitter/
3. All terminals (SA, SB (usually off), SC, GM, MD, Ops testing in Annex)
4. All terminal UPS systems (SB, SC, GM, Annex)
5. Elvis shutdown (control - power button press should be sufficient)
6. Annex UPS
7. Control Room UPS (feeds all control equip and SA)
8. Control Room Furmans (just the "Not UPSed" one is necessary)
9. SC - power everything off (can use http://scpdu1/ or unplug, power off CDs etc.)
10. All other power strips and things (walk around and look for lights)
11. Studio A, Studio Dee, Annex, Vinyl and Control AC units off
12. Lock Doors to SA and SC (in addition to Tech 1, Control, Annex)



Note: Access card systems can take 45 minutes to come online; take that into account during scheduling the outage.

This power up order should make sure LiveWire & Rivendell come up without hassle:

1.  Annex: Smooth UPS, Nick UPS, boot both
2.  Control Furman
3.  Control UPS
4.  Return to Studio A, wait for element and computer to boot
5.  If element doesn't boot, replace CMOS battery and reprogram BIOS to autostart (see ops list thread and doc)
6.  Once all systems are go on Element, check to ensure you can play music over the monitors.
7.  If right four element channels aren't online or the element is being wonky, refer to the [troubleshooting page](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Fixing_the_Board "Fixing the Board").
8.  If Studio A can broadcast and the internet is working, power transmitter on and record time. If Studio A does not come up, consider broadcasting from C.
9.  Studio C: replug, UPS, computer
10. Studio B and MD UPSs
11. Any lingering power strips.
12. Elvis backup computer (lest you get angry cron emails)

The entire shutdown sequence takes around 20 minutes (45 if the Windows machine updates take forever). Start 1 hour before outage and don't have people planning on DJing until 1-1.5 hours after. You may want to grab a flashlight from tech. Expect not to get into any card access door while the power is out, as the card reader battery backup dies quickly. Log that we're off-air to Spinitron and the [station log](https://wiki.wmfo.org/Operations/Regulatory/Station_Log "Station Log") afterwards. Best practice is to lock Studios A and C while they are offline (the "technologically confident" DJs will begin to throw switches haphazardly).
