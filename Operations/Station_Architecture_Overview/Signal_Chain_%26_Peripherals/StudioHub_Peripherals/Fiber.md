This page documets the fiber connections from Control in Curtis to the
4th floor HVAC closet in Ballou ("the tower") where the transmitter is
located. In both locations we have a 6-line trunk down to the basement;
only 5 are connected end-to-end. All fiber is 62.5/125 multimode and
maintained by Tufts Datacom. The run is estimated at between 1.0km and
1.5km.

The term "fiber box" may refer to either the beige "wall box," which
holds the 6 ST connections on the fiber trunk, or a
"[fibox](http://www.netsys-direct.com/product_p/nm-102kit.htm "http://www.netsys-direct.com/product_p/nm-102kit.htm")",
a converter between a single strand of fiber and ethernet, made by
netsys. All fiber lines require a fibox, an SFP in a switch, or a NIC in
a computer, as these hold the laser and reciever. Each of these needs to
be rated for 100 megabit over 2km on multimode; gigabit over 220m will
not connect. The SFPs we are using are Cisco GLC-FE-100FX units ... and
while they have not been cooperating fully they do connect.

The fiber lines are critical infrastructure as they connect the studio
to the transmitter (by way of a router selector), as well as ethernet
[telemetry](https://wiki.wmfo.org/Operations/Regulatory/Telemetry "Telemetry"),
a PDU, and (one day) a server. The primary connection is between two
Cisco Catalyst 2960G switches.

### Strands 

-   The **Curtis Number (C\#)** is the number on the wall box in
    Control, in English reading order
-   The **Ballou Number (B\#)** is the number on the wall box in Ballou,
    in English reading order
-   The **Strand Number (S\#)** is the number on the fiber jumpers as
    installed by Datacom. Strands 1&2 are a pair, as are 3&4.
-   The **dB loss** is measured by Datacom and noted on the device end
    of the Curtis jumpers.
-   The **Range** refers to numbers on the box end of Datacom's jumpers.
    We're not sure what they mean.
-   NC = not connected

  --------- --------- --------- ------------------- ------------- ------------------- --------- --------------- ------------- -----------------
  **C\#**   **B\#**   **S\#**   **Curtis Device**   **dB loss**   **Ballou Device**   **Via**   **Connector**   **Range**     **Direction**
  1         4         1         CONS1               9.71          TOWS1               SFP       duplex LC       14.96-11.06   Curtis → Ballou
  2         3         2         CONS1               9.27          TOWS1               SFP       duplex LC       12.61-21.5    Ballou → Curtis
  6         2         3         CONS2               13.95         NC                  FIBOX3    Simplex SC      16.34-24.1    Curtis ↔ Ballou
  4         5         -         CONS1               ?             TOWRS1              FIBOX1    simplex SC      -             Curtis ↔ Ballou
  5         6         -         -                   NC            -                   -         -               -             -
  3         1         4         CONS2               8.68          TOWET1              FIBOX2    Simplex SC      16.69-19.66   Curtis ↔ Ballou
  --------- --------- --------- ------------------- ------------- ------------------- --------- --------------- ------------- -----------------

Note that Datacom swapped strands 3&4, which have been swapped back in
Control to a working connection (tested over netsys fiboxes). However,
the dB loss for the lines is likely flipped from what is reported above.

### Curtis Connections 

  Strand (Curtis Number)   Interface         Device
  ------------------------ ----------------- ----------------------------------
  1,2                      Cisco SFP (N/C)   Cisco 2960 8 Port (N/C)
  3                        Fibox 2           Ethernet Telemetry
  4                        Fibox 1           Airfeed
  6                        Fibox 3           Tower Server (to be built/moved)

### Saturation tests 

Saturation tests can be done using `iperf -s|-c IP `run on Duke (for
CONS1) and a laptop connected to TOWS1. 

### Fiber resources 

-   [Single Mode vs. Multi-Mode: What’s the
    Difference?](http://www.imakenews.com/drs/e_article001146955.cfm "http://www.imakenews.com/drs/e_article001146955.cfm")
-   [Fiber Polarity
    Simplified](http://www.ampnetconnect.com/documents/WHITEPAPER_Fiber_Polarity_Simplified_090813.pdf "http://www.ampnetconnect.com/documents/WHITEPAPER_Fiber_Polarity_Simplified_090813.pdf")
-   [Fiber
    Connectors](http://www.fiberoptics4sale.com/Merchant2/fiber-optic-connectors.php "http://www.fiberoptics4sale.com/Merchant2/fiber-optic-connectors.php")
    - see duplex LC, ST, SC
-   [SFP
    transciever](http://en.wikipedia.org/wiki/Small_form-factor_pluggable_transceiver "http://en.wikipedia.org/wiki/Small_form-factor_pluggable_transceiver")
    - between switch and LC connector, the part with the lasers

1.  1. [Strands](#Strands)
2.  2. [Curtis Connections](#Curtis_Connections)
3.  3. [Saturation tests](#Saturation_tests)
4.  4. [Fiber resources](#Fiber_resources)

