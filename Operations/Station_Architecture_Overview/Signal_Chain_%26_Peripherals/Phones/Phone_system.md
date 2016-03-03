WMFO has two phone lines for DJs, whose inetgration into the LiveWire
network is described here. It also has a phone line to the transmitter.

### Current System {.editable}

#### Instructions to DJs {.editable}

To **answer the phone**, press the phone button once it lights up. Then
hold talkback, press preview, then release both buttons. Then talk to
the caller off-air.

To **put the caller on air**, put the phone fader *and mic 1* on and up.

To **hang up**, press the phone button again, and turn off preview.

To **dial out from the board**, press the phone button, dial on the
board’s keypad on the right, and then press the Enter button by the
arrow keys. It’s a Tufts line, so you’ll need to dial 9 to get out, and
there’s no long distance.

Please note that the lines cannot be on the board in Studio A and Studio
C simulataneously.

#### Operations documentation {.editable}

The phone system requires Euro-style faders with four buttons above
ON/OFF. We have 4 of these faders on the Studio A board and 2 on the
Studio C board. On each they are on the right side. Phones can only be
assigned to these faders.

Instead of fader numbers, the phone line faders display a status symbol.
A dot means the line is not ringing. A square means the phone is on but
not connected. A pulsing square means the line is ringing. A downward
arrow means the line is connected. An x means something is wrong, most
likely that the line is on the other board.

The system itself is the Telos Nx6, installed November 2012 in the far
side of the Control rack. See Telos documentation for more details.

 

The lines installed into the POTS wall jacks in Control have two female
ports on the other end. On each, one goes to  the Nx6 (with 3801 going
through the telemetry modem first) and the other goes to the phone
flashers. The flashers in Studio A are phones, from the perspective on
the phone lines. A single ethernet cable carries both lines into A.

### Old system {.editable}

The old phone system consisted of custom board of voicecoils and cable
connectors, and two rackmount hybrids. These were connected via
XLR-to-ethernet dongle to CONA1, which was configured to receive two
sources/destinations on one input/output RJ-45. The sources were set to
Live Mono (and a gain of 12dB). The destinations were To source: Dual
Mono. The custom board requires a power supply, and also has connectors
for lines in, lines out to flashers, TRS out the hybrids, and an
attached GPIO ethernet line that used to go to P1 8.

To answer the phone on the old system, one would hold talkback, press
preview, and release, and then turn the fader on.

### Blue-sky spec {.editable}

This is the wish list of the phone system written up before we had
settled on a specific unit.

The first stage of the upgrade is how the phone lines are routed to the
board. The new system **must**:

-   Keep the existing functionality of two lines as LiveWire streams
    with GPIO control and flashers in A
-   Extend this functionality to Studio C (only the flashers will take
    effort)
-   Allow DJs in A and C to place a call from the board using the
    numeric keypad
-   Use the same headphones and microphone as the DJs use for other
    audio
-   Not require custom-made hardware, other than cabling
-   Be maintainable without a local expert (be robust)
-   Not interfere with telemetry (wait until we have ethernet telemetry)
-   Be compatible with other plans for the phone system (voice menu,
    rotating ops contact, VoIP, etc.)
-   Fit our budget

 

The new system **should** do as many of the following as possible:

-   Fit our budget with room to spare
-   Provide DJs with caller ID
-   Maximize audio quality by minimizing conversions
-   Provide an intercom between A and B (B phone needs to be installed)
-   Support future growth

1.  1. [Current System](#Current_System)
    1.  1.1. [Instructions to DJs](#Instructions_to_DJs)
    2.  1.2. [Operations documentation](#Operations_documentation)

2.  2. [Old system](#Old_system)
3.  3. [Blue-sky spec](#Blue-sky_spec)

