This page hosts a running list of short term and long term Operations
Department projects, as well as suggestions which may or may not be
undertaken. It services primarily as a place for the Ops Director and
other station leadership to write down all the different jobs on the
horizon. If you are not a member of the ops department but have a
suggestion about future projects that you feel would be beneficial,
email the [ops
list](https://wiki.wmfo.org/Staff_Info/Staff_Newsgroups "Staff Newsgroups").

Projects specification should be fairly specific. This is not the place
for broad feature requests without specific implementation plans. All
suggestions should link generously to source that would provide good
starting points for undertaking such a project.

We try to keep this page updated, but it's not crazy updated. Ask the
ops director for the lastest info.

Short Term ToDo {.editable}
---------------

Projects with components currently underway or scheduled for completion
in the next 6 months. Within each subheading, items are listed in the
order they should be done, either by dependency or priority (sometimes).
Between subheadings, items are largely independent.

The number 1 ops priority is to fix any existing systems that break.

 

### Nick's List {.editable}

1.  Print out RF report and transmitter report: replace Radiation
    exposure signage
2.  Circuit breaker in DJ outlet
3.  Transmitter poweroff DJ button
4.  Migrate wiki off of mindtouch
5.  New website theme
6.  DJ portal
7.  Automation MD selected
8.  update inventory
9.  Website Theme Refresh
10. Duke FLAC archive
11. Control UPS Batteries
12. Water Filter Thing
13. UPS Networking and Policies
14. VoIP
    1.  NX6 line duplication for Studio C

15. Ringo to tower (new card)
16. Super to ZFS
17. Shoutcast V2 streaming VM on new Duke
18. Clean up and organize filesystems (See Duke /home/wmfo-admin/)

### To Buy {.editable}

-   [Second Storage
    Server](http://www.thinkmate.com/system/rax-xs8-1260v3 "http://www.thinkmate.com/system/rax-xs8-1260v3")
-   6TB drive set (x10)
-   [New duke with
    IPMI](http://www.thinkmate.com/system/rax-xs4-1160v3 "http://www.thinkmate.com/system/rax-xs4-1160v3")
-   PCI-E ASI Card
-   New B Terminal (thinkmate)
-   New MD Terminal (thinkmate)
-   All the furniture
-   Color Laser
-   Water bubbler
-   New 8 channel compressor
-   500 series everything
-   Stands, mics
-   Headphone monitor solution for Dee
-   2000 CD-Rs

#### Facilites {.editable}

-   Improve [MD sticker
    dispenser](https://groups.google.com/d/topic/wmfo-ops/6vWPCxxavFc/discussion "https://groups.google.com/d/topic/wmfo-ops/6vWPCxxavFc/discussion")

#### Equipment {.editable}

-   Review and modify UPS and auto power-up/down settings and systems
-   ~~~~Studio C - Set up ~~Automation Scheduler~~ (loads logs generated
    by Tinmachine), Rivendell-Spinitron Update (maybe)~~~~
    -   One day: switch to digital audio I/O
-   Research and install phone menu system - All - 2013 (meh?)
-   Build and configure GM computer - Or not.

#### Tower {.editable}

-   Power
    -   Document tower
-   Tidy up
    -   Take photos for reference, insurance
    -   Replace radiation explosure signage
-   Purchase, build, configure, install, test tower server - Now!
-   Silence detection and automatic failover - next fall or spring

#### System Software {.editable}

-   Set up Pathfinder to detect silence
-   Document and review backup system - 2013
    -   Automatic Wiki backups, regular backups to tower server
-   Document archive and streaming system - Max
-   [Automatically clean home
    folders](https://groups.google.com/d/topic/wmfo-ops/0PAB15Ct3SA/discussion "https://groups.google.com/d/topic/wmfo-ops/0PAB15Ct3SA/discussion")

#### In-House Software {.editable}

-   Fix bugs, test, and redeploy as necessary
-   ~~[Watchdog](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Watchdog "Watchdog")
    and
    [Rivendell-Spinitron](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Rivendell_-_Spinitron_Update "Rivendell - Spinitron Update"):
    test and redeploy~~
-   [Automatic
    import](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Automatic_CD_Import_System "Automatic CD Import System"),
    version 3:
    -   Revise File Sanitizer and Importer - Max
    -   ~~Rewrite Lyrics Flagger - Connor~~
        -   Version 1 is done. Need to add more sites.
-   Volunteers' Song Flagger
-   [Automation
    scheduler](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Automatic_Rivendell_Log_Generation "Automatic Rivendell Log Generation"):
    play music that DJs play (no metal)
-   Manual Song Flagger - Max
-   New Studio C scheduler - Ross?
    -   Digitize everything while you're at it, says Jameelah
-   Update Rivendell-Spinitron to log only from air studio - Max
-   [DJ
    Portal](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/DJ_Portal "DJ Portal")
    - Nate
-   Review, document, and git(hub)-ify all other code (order TBD)
-   Automatic ops-list e-mail notification system for watchdog, syslog,
    and other critical error detection systems
-   Automatic silence detect and notification/correction system
    (see [here](https://groups.google.com/forum/?fromgroups=#!searchin/wmfo-ops/silence$20detection/wmfo-ops/xgi29gPGHb4/tza7liojeS8J "https://groups.google.com/forum/?fromgroups=#!searchin/wmfo-ops/silence$20detection/wmfo-ops/xgi29gPGHb4/tza7liojeS8J") and [here](https://groups.google.com/forum/?fromgroups=#!searchin/wmfo-ops/silence$20detect/wmfo-ops/-W5WQwYnTck/dp_ejtYDxbsJ "https://groups.google.com/forum/?fromgroups=#!searchin/wmfo-ops/silence$20detect/wmfo-ops/-W5WQwYnTck/dp_ejtYDxbsJ") and [here](https://groups.google.com/forum/?fromgroups=#!searchin/wmfo-ops/silence$20detect/wmfo-ops/sZIKt4ITPe8/xnd9o5KUTMQJ "https://groups.google.com/forum/?fromgroups=#!searchin/wmfo-ops/silence$20detect/wmfo-ops/sZIKt4ITPe8/xnd9o5KUTMQJ") and [here](https://groups.google.com/forum/?fromgroups=#!searchin/wmfo-ops/silence$20detect/wmfo-ops/e7A3Vc70e0c/6VdOMApiCqUJ "https://groups.google.com/forum/?fromgroups=#!searchin/wmfo-ops/silence$20detect/wmfo-ops/e7A3Vc70e0c/6VdOMApiCqUJ"))

#### Web-specific Projects {.editable}

-   Refresh website layout - Nate, Nick, Sam - summer
    -   Re-work homepage: possible splash page
    -   Change backgroud
    -   Make links, navigation more intuitive? 
    -   Contact page
    -   Better blogging categories (work with New Media on this one)
    -   Improve mobile layout
-   Improve Shoutcast experience - Nate
    -   Upgrade to SHOUTcast 2.0 or IceCast -
        [http://www.shoutcast.com/broadcast-tools](http://www.shoutcast.com/broadcast-tools "http://www.shoutcast.com/broadcast-tools")
    -   Increase simultaneous streaming limit
    -   Allow listeners on website to choose stream quality
-   Switch [WMFO webstream metadata
    system](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/SHOUTcast_Metadata_Updater "SHOUTcast Metadata Updater")
    to use Spinitron Push
-   Last.fm integration - Connor
-   Show reccomender - Nate
-   [Fix redirect
    pages](https://groups.google.com/forum/?hl=en&fromgroups#!topic/wmfo-ops/-bjxkGTkh7E "https://groups.google.com/forum/?hl=en&fromgroups#!topic/wmfo-ops/-bjxkGTkh7E")
-   Online show forms. Ben has done the
    [front](https://wiki.wmfo.org/forms.wmfo.org/form.html "forms.wmfo.org/form.html")
    [end](https://wiki.wmfo.org/forms.wmfo.org/form2.html "forms.wmfo.org/form2.html") -
    2013 - with PD

#### Other {.editable}

-   ~~Create training videos on Rivendell, the board, the phones - Max
    and Nick~~ Completed by Ben Stern
-   Add OTT IDs to Rivendell - Edward
-   Talk to Tom at Spinitron about cleaning up autocomplete DB
-   Document donations website and donations drive best practices -
    early 2013
-   Improve Google Docs organization. Beware different folders have
    different permissions. - Alex
-   Improve wiki documentation and organization - Alex

 

#### Big Purchases for FY14 {.editable}

-   Tower server
-   RDS
-   New Headphone StudioHub
-   A/C for Dee and Vinyl Library
-   Modulation Monitor
-   Mic preamps etc for B
-   Carpet?

Long Term ToDo {.editable}
--------------

Not yet launched and unscheduled projects with no set completion dates.
Not all of these are worth doing; consult the ops list if uncertain.

-   Online studio A [kill
    switch](https://groups.google.com/d/topic/wmfo-ops/JM3J_n6jGaA/discussion "https://groups.google.com/d/topic/wmfo-ops/JM3J_n6jGaA/discussion") (just
    use VNC to duke-rivendell)
-   Switch Windows 2008 servers (Super+Smooth) to Linux with Windows VMs
    as necessary (Fa2014/Ross)
-   Red trims on non-hallway or Studio A doors and windows (lounge,
    vinyl library)
-   Move wiki off of MindTouch Core [due to
    EOL](https://groups.google.com/forum/?fromgroups#!topic/wmfo-ops/9iZ1829mwhY%5B1-25%5D "https://groups.google.com/forum/?fromgroups#!topic/wmfo-ops/9iZ1829mwhY%5B1-25%5D").
    (if it ain't broke...)
-   Studio B Axia Board + Complete Axia System (not sure of utility or
    available space)
-   Flooring:
    -   Studio B - New Carpet
    -   Studio Dee Floor Repair + New carpet
    -   Vinyl Library + Annex + Studio C - New carpet
    -   Hallway - New Carpet
    -   Lounge + Offices - New carpet
    -   Back Hallway + Storage + Bathrooms + Tech 1&2 - Floor Repair
-   Consider switching to a bug/work tracking system like
    [RT](http://bestpractical.com/rt/ "http://bestpractical.com/rt/") as
    opposed to this page
-   New station-wide AC system to replace current, aging system (window
    in A, need windows in Dee and Vinyl)
-   Replace final swipe-style door readers (front door and stairs door)
    with prox-style readers (maybe w/ co-funding from Public
    Saftey--let's not)

1.  1. [Short Term ToDo](#Short_Term_ToDo)
    1.  1.1. [Nick's List](#Nick's_List)
    2.  1.2. [To Buy](#To_Buy)
        1.  1.2.1. [Facilites](#Facilites)
        2.  1.2.2. [Equipment](#Equipment)
        3.  1.2.3. [Tower](#Tower)
        4.  1.2.4. [System Software](#System_Software)
        5.  1.2.5. [In-House Software](#In-House_Software)
        6.  1.2.6. [Web-specific Projects](#Web-specific_Projects)
        7.  1.2.7. [Other](#Other)
        8.  1.2.8. [Big Purchases for FY14](#Big_Purchases_for_FY14)

2.  2. [Long Term ToDo](#Long_Term_ToDo)

