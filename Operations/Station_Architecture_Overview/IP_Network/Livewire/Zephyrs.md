*Current status:* The WiFi dongle is not cooperating.  The mobile unit
has a bad XLR input. Otherwise the Zephyrs are in working order and we
are capable of remote broadcast.

The Zephyr / IP units allows us to do remote broadcasts. The system
consists of two units. The stationary unit is mounted in Bay B, between
Control and Studio A. The mobile unit resides in Storage when not in
use. The units can "call" each other over the internet, and send audio
in each direction.

Log 
---

Log uses and test calls of the Zephyrs here and report any problems.
This allows us to make sure test calls happen often enough.

  Date      Event                            Notes
  --------- -------------------------------- -----------------------------------------------
  11/6/12   Election Night @ Campus Center   Wired connection held high bitrate for hours.
  3/30/13   Ops meeting                       

 

  
-

Remote Broadcasting 
-------------------

If you just want to have up to 4 people talking with mics headphones,
you don't need any other equipment. The Zephyr supports 4 XLR inputs
(only 3 are working) and 4 monitors (headphones with 1/4" jacks; one on
the front, three on the back). The knobs on the top row control the
input volume, while buttons toggle sending that input to XLR output A or
B, i.e. speakers. You'll probably want every active mic on A and B.
There is no way to control the volume going to the speakers, nor what
input (it gets all 4 plus Livewire receive). Each monitor has its own
volume and the option of whether to listen to send, receive, both, or
neither. Again, you'll probably want both, which will let you talk to
someone in the studio. While simpler, this setup is the one you're less
likely to use.

If you want more control, bring the mobile Allen and Heath (a ZED 14
that lives in the big hard Gator case in tech 2) and optionally the Rane
headphone splitter (1RU unit in tech 2) although the Zephyr's monitors
should be plenty. Run the A&H main out to Zephyr inputs 2 and 3 (1 does
not work properly). On the Zephyr, A is L and B is R; assign inputs 2
and 3 to match the wiring from the A&H and make sure their gain knobs
are turned up.

Normally you'd put all your mics on the A&H but if you ever want to put
them directly into the Zephyr, there's a setting to turn up their gain.
Set it back to pro audio when you're done, otherwise it will sound
horrible from having so much gain.

In either setup, bring the longest ethernet cable you can find (it
typically lives on top of the mobile Zephyr in Storage). Bring plenty of
XLRs (1 per mic or speaker; 2 to connect A&H out to Zephyr; spares);
power cables (1 per Zephyr, speaker, or A&H); headphones mics stands and
holders (1 per person). Bring the swag box, which has a roll of gaffer's
tape to tie down cables and put up the banner. Make sure in advance
you'll have a table, or bring one. Bring a laptop and charger to log
Spinitron from. Even if you're just talking for more than a few minutes,
log something and set the format as "Live". You still need to log and
you still need to do station IDs, but the PD may waive the PSA
requirement.

There is no way to "preview" only certain audio from the Zephyr; it's
only one stream. If remote and studio DJs need to talk off-air, and you
don't want to use a normal phone, the studio DJ should put another
source on-air but take it off Program 3 (i.e. not send it to the
remote), take mic 1 and the Zephyr off Program 1 (i.e. off-air), preview
the Zephyr fader and turn mic 1 on and up.

The mobile unit needs internet connectivity, which can happen in one of
three ways: the built-in ethernet jack, the USB WiFi dongle taped to the
unit, and a cellular data dongle (boxed in Storage, used a few times in
2011, [Clear](http://www.clear.com/ "http://www.clear.com/") data plan
required). Both the ethernet and WiFi dongle should connect to the Tufts
network DHCP automatically (the Link and Z/IP indicators onscreen should
be green). From there, press the CONN button of the right of the front
panel and call the most recent number, which should be the stationary
unit. Make sure it has the `tscp:` prefix. In practice, try to use the
Ethernet cable (we have a pretty long one).

In the station, bring up the Remote Broadcast profile on the Studio A
Element. It's identical to the default profile (as of 10/12) except the
DJ Mixer has been replaced with the Zephyr, and all other faders go to
Program 3 (as well as Program 1), creating a mix-minus to send to the
remote unit. Put up the Zephyr fader like any other.

If you're running the mobile unit over Tufts wired connection, you can
crank minimum and maximum bitrates from the 128, 192 default to 256 for
both (it won't save higher values). The decoder buffer has defaults of
3(min) and 4(max) seconds. You can experiment dropping these, turning
them back down if you experience choppiness indicating dropped packets.
Put them back on the defaults when you're done.

Test Calls 
----------

Make test calls *more frequently than every 6 months*. (This ensures all
the registrations are kept current.) Make a test call between the units
*a week before a remote broadcast event*. (This way there is time to
troubleshoot if something goes wrong, and so everyone knows who the
system works.)

Call the Telos test line from the stationary unit, the mobile unit over
WiFi, and the mobile unit over ethernet. (If you're planning on using
the cell dongle, make sure that works too.)

Set up the mobile board with some input, wire it to the mobile Zephyr,
and call the stationary unit. See that the call goes through. Add the
appropriate channel to the Studio A board. Preview on that channel. If
the audio you're feeding into the mobile board comes through the DJ
headphones, you're all set. If not, contact the ops list.

Troubleshooting 
---------------

If the Zephyrs haven't been used in longer than six months, start from
scratch and do the following.

If the stationary unit displays a green "Link" indicator but a red
"Z/IP" indicator, do a factory reset (Settings -\> Reboot -\> Reset to
Defaults). Follow along in the manual's quickstart guide (google for the
latest version). Best practice is to unplug the ethernet cable first in
case the IP it chooses conflicts with one we use. Go to
Network-\>Ethernet config. Barring massive changes to LAN [IP
table](https://wiki.wmfo.org/index.php?title=Operations/Diagrams_%26_Tables/IP_Address_Space "IP Address Space")
after this writing, the IP is 192.168.0.140, the netmask is 255.255.0.0,
the gateway is 192.168.0.10, and the DNS is 8.8.8.8 (Google). Disable
DHCP. Activate the settings. Plug in the ethernet cable. The Link and
Z/IP indicators should now be green, and you should be able to call the
Telos test server. If not (and Link is green), contact the ops list or
Telos support.

Set up the group, which you may need to recreate, using the [old
credentials](https://wiki.wmfo.org/Operations/Credentials/Internal_Credentials#Zephyr_IP_Unit "https://wiki.wmfo.org/Operations/Credentials/Internal_Credentials#Zephyr_IP_Unit"). You
can use the browser web interface to change the unit password and the
listen port to 9636. Change the Livewire Source to 10400 and the
destination to 10502 (Pgm3@CONSE1).

The stationary unit is CONZP1 and the mobile unit is MOBZP1.

At one point we had the Zephyr MACs registered as "assests", which would
last for 7 years and be independent of an individual. Neat trick if you
can manage it. Otherwise [manually
register](http://it.tufts.edu/nonreg "http://it.tufts.edu/nonreg") the
MAC addresses yourself. Once that's done, plug in the cable or dongle to
the mobile unit, do the network config (enable DHCP), and select that
source as the "streaming source". Same deal as above: The Link and Z/IP
indicators should now be green, and you should be able to call the Telos
test server. If not (and Link is green), try doing a factory reset. If
there's still an issue, contact the ops list or Telos support.

Once you have two units that can each call the Telos test server, you
should be able to call one from another using the groups you set up.
It's sufficient for now to look at each unit and see that they both
think they're connected.

There are a bunch of audio settings that may need attention. Consult the
engineers or ops list. Then do the test call procedure as above. And
then you can say that it works.

Addendum: The stationary unit has only a LAN IP and requires port
forwarding. The D-Link router should be set up to forward ports 24308
(default port for Telos's server) and 9636 ("our port", what the Zephyr
is told to listen to for incoming calls from the mobile unit). Your
shouldn't need to modify these.

1.  1. [Log](#Log)
2.  2. [ ](#)
3.  3. [Remote Broadcasting](#Remote_Broadcasting)
4.  4. [Test Calls](#Test_Calls)
5.  5. [Troubleshooting](#Troubleshooting)

