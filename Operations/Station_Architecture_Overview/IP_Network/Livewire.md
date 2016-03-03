Livewire's Layers of Abstraction {.editable}
--------------------------------

Livewire is an Audio over IP standard. Basically it allows any device on
the network to access any stream, regardless of the location (so a
router selector node can pull up the microphone in Studio A from Ballou
and listen to it).

In general, all Livewire interface happens through proprietary dedicated
devices. These perform one of two functions:

1.  A node performs a bridge between a standard protocol (analog
    balanced audio, digital AES audio, or PCM digital audio inside our
    computer in the case of the ASI card) and the Livewire network.
    Basically, this bridges standard non-Livewire audio with a fully
    routable Livewire stream.
2.  Several devices do processing on solely Livestream audio, so both
    input and output are Livewire streams. Examples of these are the
    Studio Engine and the Omnia audio processors (though the Omnia has
    support for digital audio output directly).

Problems with IP Audio {.editable}
----------------------

One of the critical issues with IP-based audio has to do with latency.
Packetized data transmission enables very flexible routing and delivery,
but is a "best effort" system. If the amount of data to be sent exceeds
the capacity of the channel or the buffer, data will be dropped
indiscriminantly. To account for this, protocols exist which guarantee
delivery of data (TCP) over unreliable channels. However, this can
increase the latency of the channel.

Livewire requires Quality of Service (QoS) configuration to prioritize
its traffic. This means that the network switch can discriminate between
Livewire streams and other network traffic. In such a fashion, the
switch will drop standard data packets (like your browser HTTP
connection to Facebook) before it drops Livewire packets, thus
prioritizing reliability of the Livewire stream over standard traffic.

This is not a perfect system: it is still possible for interference to
garble packets, but in practice in a small and well-constructted network
like ours (read: actual CAT6 cables and not chinese garbage), the effect
of this will be minimal and it is accounted for by the protocol. There
is still delay associated with the encoding, packetization, and
transmission but by minimizing this using the above techniques we get a
very reliable and flexible audio system.

 

Livewire is the porotcol that all Axia/Telos equipment uses. For more
information see *Introduction to Livewire* and other
[manuals](http://axiaaudio.com/manuals "http://axiaaudio.com/manuals")
published by Axia.

*Inputs* and *Outputs* on the Nodes and PowerStations are the actual
ethernet (specifically shielded cat5e) cable connection. Each Node has
eight of each. These usually translate directly to *sources*
and *destinations*, although it's possible to have one physical line
carry two source or destinations' worth of data. Sources are also
produced internally, e.g. Program 1 from an Element.

Audio in the network is in the form of a *stream*. Streams are
identified by both a name and a channel number. Streams must have
exactly one source but may be routed to any number of destinations. The
name and channel number are assigned at the source, the latter by [WMFO
convention](https://wiki.wmfo.org/index.php?title=Operations/Diagrams_%26_Tables/LW_Address_Space "LW Address Space").
Streams are global to the WMFO LAN.

So far we've disucussed the Livewire network; the next two layers are
specifically part of the Element control board. *Source Profiles* bundle
a source with control data. *Show Profiles* map source profiles to
physical faders. Both types of profile are local to one Element and are
described in chapters 3 and 6 of the Element manual, respectively.

1.  1. [Livewire's Layers of
    Abstraction](#Livewire's_Layers_of_Abstraction)
2.  2. [Problems with IP Audio](#Problems_with_IP_Audio)

