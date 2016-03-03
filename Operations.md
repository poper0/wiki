This page is designed to facilitate the ops learning process. There's a
lot of information to know, most of which is not covered in any Tufts
course. However, knowing how this station operates will give you a lot
of practical, real world experience in:

1.  Network administration and Networking
2.  Linux System Administration
3.  Axia/Livewire configuration
4.  Hackery

The [Operations
Director](/About_WMFO/Executive_Board/Operations_Dept. "Operations Dept.") (or
any former Operations Directors) are great starting points if you have
trouble finding information, but you can find most of what there is to
know within this Wiki.

Here is your crash course wiki curriculum:

1.  Station Architecture
    1.  Overview
    2.  Livewire Architecture
    3.  Server Architecture
        1.  Primary Hypervisor
            1.  Rivendell VM
            2.  Web host VM
            3.  Webstream VM
            4.  Scripts/misc VM - email relay, telemetry, SMTP, SSH key
                propogator
            5.  Sandbox VM

        2.  Primary storage node
        3.  Secondary storage node
        4.  Backup node

2.  Signal Chain Overview
    1.  Analog/Digital Nodes
    2.  StudioHub
    3.  ASI Card (inside Duke)
    4.  EAS
    5.  Element/Studio Engine (Studio A)
    6.  Power Station (Studio C)
    7.  Omnias
    8.  Transmitter
    9.  Modulation Monitors

3.  Other devices
    1.  PDUs
    2.  CD Players
    3.  Amplifiers

 

This section details tables and explanations related to the ops
department. Some of this content is accessible only by logging in with
an account of the appropriate credential level. The best way to get
information is to contact the ops list,
[wmfo-ops@googlegroups.com](mailto:wmfo-ops@googlegroups.com "wmfo-ops@googlegroups.com") and
be trained by existing ops volunteers.

 

The [Rivendell](https://wiki.wmfo.org/Operations/Rivendell "Rivendell")
page provides a good overview of the [signal
chain](https://docs.google.com/a/wmfo.org/drawings/d/1ZioPk_CP5EZg8U6Jix9IY1ol_1xH6u0A_kD7RZt3h1g/edit "https://docs.google.com/a/wmfo.org/drawings/d/1ZioPk_CP5EZg8U6Jix9IY1ol_1xH6u0A_kD7RZt3h1g/edit").
[LiveWire](https://wiki.wmfo.org/Operations/Axia_and_Telos "Axia and Telos")
is the protocol that routes audio through the station, and is used by
all Axia equipment (and their parent company, Telos). You can get a
sense of the network from the
[I](https://wiki.wmfo.org/index.php?title=Operations/Diagrams_%26_Tables/IP_Address_Space "IP Address Space")[P
table](https://wiki.wmfo.org/index.php?title=Operations/Diagrams_%26_Tables/IP_Address_Space "IP Address Space") and
and get details from the [normal
tables](https://wiki.wmfo.org/index.php?title=Operations/Diagrams_%26_Tables/Axia_Normal_Tables "Axia Normal Tables").
Most of our code is or will/should be on
[Github](https://github.com/organizations/WMFO "https://github.com/organizations/WMFO").
And sometimes you just need to [fix the
board](https://wiki.wmfo.org/Operations/Axia_and_Telos/Fixing_the_Board "Fixing the Board").

Contents 
--------

-   [Annual
    Checklist](https://wiki.wmfo.org/Operations/Annual_Checklist "Operations/Annual_Checklist")
-   [Credentials](https://wiki.wmfo.org/Operations/Credentials "Operations/Credentials")
    -   [Hosting
        Credentials](https://wiki.wmfo.org/Operations/Credentials/Hosting_Credentials "Operations/Credentials/Hosting_Credentials")
    -   [Internal
        Credentials](https://wiki.wmfo.org/Operations/Credentials/Internal_Credentials "Operations/Credentials/Internal_Credentials")
    -   [Linux Remote
        GUI](https://wiki.wmfo.org/Operations/Credentials/Linux_Remote_GUI "Operations/Credentials/Linux_Remote_GUI")
    -   [Remote
        Access](https://wiki.wmfo.org/Operations/Credentials/Remote_Access "Operations/Credentials/Remote_Access")
    -   [Service/Vendor
        Credentials](https://wiki.wmfo.org/Operations/Credentials/Service%2F%2FVendor_Credentials "Operations/Credentials/Service//Vendor_Credentials")
    -   [Tax
        Exemption](https://wiki.wmfo.org/Operations/Credentials/Tax_Exemption "Operations/Credentials/Tax_Exemption")
    -   [Tufts
        Credentials](https://wiki.wmfo.org/Operations/Credentials/Tufts_Credentials "Operations/Credentials/Tufts_Credentials")
    -   [Web2.0
        Credentials](https://wiki.wmfo.org/Operations/Credentials/Web2.0_Credentials "Operations/Credentials/Web2.0_Credentials")
-   [Historical](https://wiki.wmfo.org/Operations/Historical "Operations/Historical")
    -   [1992 Construction Permit
        Application](https://wiki.wmfo.org/Operations/Historical/1992_Construction_Permit_Application "Operations/Historical/1992_Construction_Permit_Application")
    -   [Archive & Streaming
        (old)](https://wiki.wmfo.org/index.php?title=Operations/Historical/Archive_%26_Streaming_(old) "Operations/Historical/Archive_&_Streaming_(old)")
    -   [Fall 2011 Data Server HD
        Upgrade](https://wiki.wmfo.org/Operations/Historical/Fall_2011_Data_Server_HD_Upgrade "Operations/Historical/Fall_2011_Data_Server_HD_Upgrade")
    -   [Studio A Renovation (Jan
        2011)](https://wiki.wmfo.org/Operations/Historical/Studio_A_Renovation_(Jan_2011) "Operations/Historical/Studio_A_Renovation_(Jan_2011)")
    -   [Tracker:
        wmfo.org](https://wiki.wmfo.org/Operations/Historical/Tracker%3A_wmfo.org "Operations/Historical/Tracker:_wmfo.org")
-   [Reference and
    Hacks](https://wiki.wmfo.org/Operations/Reference_and_Hacks "Operations/Reference_and_Hacks")
    -   [CD Ripper
        7601XDP](https://wiki.wmfo.org/Operations/Reference_and_Hacks/CD_Ripper_7601XDP "Operations/Reference_and_Hacks/CD_Ripper_7601XDP")
    -   [CON Wire
        Routing](https://wiki.wmfo.org/Operations/Reference_and_Hacks/CON_Wire_Routing "Operations/Reference_and_Hacks/CON_Wire_Routing")
    -   [Diagrams &
        Tables](https://wiki.wmfo.org/index.php?title=Operations/Reference_and_Hacks/Diagrams_%26_Tables "Operations/Reference_and_Hacks/Diagrams_&_Tables")
    -   [General Troubleshooting
        Checklists](https://wiki.wmfo.org/Operations/Reference_and_Hacks/General_Troubleshooting_Checklists "Operations/Reference_and_Hacks/General_Troubleshooting_Checklists")
    -   [KVM Guest
        Setup](https://wiki.wmfo.org/Operations/Reference_and_Hacks/KVM_Guest_Setup "Operations/Reference_and_Hacks/KVM_Guest_Setup")
    -   [Music
        Department](https://wiki.wmfo.org/Operations/Reference_and_Hacks/Music_Department "Operations/Reference_and_Hacks/Music_Department")
        -   [Printers](https://wiki.wmfo.org/Operations/Reference_and_Hacks/Music_Department/Printers "Operations/Reference_and_Hacks/Music_Department/Printers")
        -   [PSA Department Rivendell
            Access](https://wiki.wmfo.org/Operations/Reference_and_Hacks/Music_Department/PSA_Department_Rivendell_Access "Operations/Reference_and_Hacks/Music_Department/PSA_Department_Rivendell_Access")
    -   [On Air
        Lights](https://wiki.wmfo.org/Operations/Reference_and_Hacks/On_Air_Lights "Operations/Reference_and_Hacks/On_Air_Lights")
    -   [Power
        Tools](https://wiki.wmfo.org/Operations/Reference_and_Hacks/Power_Tools "Operations/Reference_and_Hacks/Power_Tools")
    -   [SA Arduino Control
        Panel](https://wiki.wmfo.org/Operations/Reference_and_Hacks/SA_Arduino_Control_Panel "Operations/Reference_and_Hacks/SA_Arduino_Control_Panel")
    -   [Studio A
        checklist](https://wiki.wmfo.org/Operations/Reference_and_Hacks/Studio_A_checklist "Operations/Reference_and_Hacks/Studio_A_checklist")
-   [Regulatory](https://wiki.wmfo.org/Operations/Regulatory "Operations/Regulatory")
    -   [EAS
        Machine](https://wiki.wmfo.org/Operations/Regulatory/EAS_Machine "Operations/Regulatory/EAS_Machine")
    -   [Radiation
        Exposure](https://wiki.wmfo.org/Operations/Regulatory/Radiation_Exposeure "Operations/Regulatory/Radiation_Exposeure")
    -   [Station
        Log](https://wiki.wmfo.org/Operations/Regulatory/Station_Log "Operations/Regulatory/Station_Log")
    -   [Telemetry](https://wiki.wmfo.org/Operations/Regulatory/Telemetry "Operations/Regulatory/Telemetry")
-   [Station Architecture
    Overview](https://wiki.wmfo.org/Operations/Station_Architecture_Overview "Operations/Station_Architecture_Overview")
    -   [Code](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code "Operations/Station_Architecture_Overview/Code")
        -   [Automatic CD Import
            System](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Automatic_CD_Import_System "Operations/Station_Architecture_Overview/Code/Automatic_CD_Import_System")
            -   [Filename
                Sanitizer](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Automatic_CD_Import_System/Filename_Sanitizer "Operations/Station_Architecture_Overview/Code/Automatic_CD_Import_System/Filename_Sanitizer")
            -   [LyricsFlagger](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Automatic_CD_Import_System/LyricsChecker "Operations/Station_Architecture_Overview/Code/Automatic_CD_Import_System/LyricsChecker")
            -   [Profanity-Detecting
                Regex](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Automatic_CD_Import_System/Profanity-Detecting_Regex "Operations/Station_Architecture_Overview/Code/Automatic_CD_Import_System/Profanity-Detecting_Regex")
        -   [Automatic Rivendell Log
            Generation](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Automatic_Rivendell_Log_Generation "Operations/Station_Architecture_Overview/Code/Automatic_Rivendell_Log_Generation")
        -   [DJ
            Portal](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/DJ_Portal "Operations/Station_Architecture_Overview/Code/DJ_Portal")
        -   [Donations Website (Rev.
            4/13)](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Donations_Website_(Rev._4%2F%2F13) "Operations/Station_Architecture_Overview/Code/Donations_Website_(Rev._4//13)")
        -   [Metadata
            Grabber](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Metadata_Grabber "Operations/Station_Architecture_Overview/Code/Metadata_Grabber")
        -   [Rivendell - Spinitron
            Update](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Rivendell_-_Spinitron_Update "Operations/Station_Architecture_Overview/Code/Rivendell_-_Spinitron_Update")
        -   [SHOUTcast Metadata
            Updater](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/SHOUTcast_Metadata_Updater "Operations/Station_Architecture_Overview/Code/SHOUTcast_Metadata_Updater")
        -   [Watchdog](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Code/Watchdog "Operations/Station_Architecture_Overview/Code/Watchdog")
    -   [Computers](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers "Operations/Station_Architecture_Overview/Computers")
        -   [Archives](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/Archives "Operations/Station_Architecture_Overview/Computers/Archives")
        -   [Backups](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/Backups "Operations/Station_Architecture_Overview/Computers/Backups")
        -   [Data
            Store](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/Data_Store "Operations/Station_Architecture_Overview/Computers/Data_Store")
        -   [Generic Computer
            Setup](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/Generic_Computer_Setup "Operations/Station_Architecture_Overview/Computers/Generic_Computer_Setup")
        -   [Power
            Sequence](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/Power_Sequence "Operations/Station_Architecture_Overview/Computers/Power_Sequence")
        -   [Public Website Back End
            Access](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/Public_Website_Back_End_Access "Operations/Station_Architecture_Overview/Computers/Public_Website_Back_End_Access")
        -   [Public Website
            Side-Banner](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/Public_Website_Side-Banner "Operations/Station_Architecture_Overview/Computers/Public_Website_Side-Banner")
        -   [Ringo - Primary
            Fileserver](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/Ringo_-_Primary_Fileserver "Operations/Station_Architecture_Overview/Computers/Ringo_-_Primary_Fileserver")
        -   [SmoothCriminal](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/SmoothCriminal "Operations/Station_Architecture_Overview/Computers/SmoothCriminal")
        -   [SSL
            certificates](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/SSL_certificates "Operations/Station_Architecture_Overview/Computers/SSL_certificates")
        -   [SuperTramp](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/SuperTramp "Operations/Station_Architecture_Overview/Computers/SuperTramp")
        -   [ThinWhiteDuke](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/ThinWhiteDuke "Operations/Station_Architecture_Overview/Computers/ThinWhiteDuke")
        -   [Tupac](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/Tupac "Operations/Station_Architecture_Overview/Computers/Tupac")
        -   [Wiki](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Computers/Wiki "Operations/Station_Architecture_Overview/Computers/Wiki")
    -   [Electrical
        Power](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Electrical_Power "Operations/Station_Architecture_Overview/Electrical_Power")
        -   [AC Electrical
            Service/AC](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Electrical_Power/AC_Electrical_Service%2F%2FAC "Operations/Station_Architecture_Overview/Electrical_Power/AC_Electrical_Service//AC")
        -   [PDU
            Manipulation](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Electrical_Power/PDU_Manipulation "Operations/Station_Architecture_Overview/Electrical_Power/PDU_Manipulation")
    -   [IP
        Network](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network "Operations/Station_Architecture_Overview/IP_Network")
        -   [IP Address
            Space](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/IP_Address_Space "Operations/Station_Architecture_Overview/IP_Network/IP_Address_Space")
        -   [Livewire](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire "Operations/Station_Architecture_Overview/IP_Network/Livewire")
            -   [Axia Normal
                Tables](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables "Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables")
                -   [CONA1](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/CONA1 "Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/CONA1")
                -   [CONASI1](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/CONASI1 "Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/CONASI1")
                -   [COND1](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/COND1 "Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/COND1")
                -   [SAA1](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/SAA1 "Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/SAA1")
                -   [SBA1](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/SBA1 "Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/SBA1")
                -   [SBD1](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/SBD1 "Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/SBD1")
                -   [SCPSA1](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/SCPSA1 "Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/SCPSA1")
                -   [SCPSM1A](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/SCPSM1A "Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Normal_Tables/SCPSM1A")
            -   [Axia Routing
                Reading/Manipulation](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Routing_Reading%2F%2FManipulation "Operations/Station_Architecture_Overview/IP_Network/Livewire/Axia_Routing_Reading//Manipulation")
            -   [Dumping a Livewire
                Stream](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Dumping_a_Livewire_Stream "Operations/Station_Architecture_Overview/IP_Network/Livewire/Dumping_a_Livewire_Stream")
            -   [Fixing the
                Board](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Fixing_the_Board "Operations/Station_Architecture_Overview/IP_Network/Livewire/Fixing_the_Board")
            -   [LW Address
                Space](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/LW_Address_Space "Operations/Station_Architecture_Overview/IP_Network/Livewire/LW_Address_Space")
                -   [SCPSM1PM](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/LW_Address_Space/SCPSM1PM "Operations/Station_Architecture_Overview/IP_Network/Livewire/LW_Address_Space/SCPSM1PM")
            -   [Webstream Omnia
                One](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Webstream_Omnia_One "Operations/Station_Architecture_Overview/IP_Network/Livewire/Webstream_Omnia_One")
            -   [Zephyrs](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/IP_Network/Livewire/Zephyrs "Operations/Station_Architecture_Overview/IP_Network/Livewire/Zephyrs")
    -   [Rivendell](https://wiki.wmfo.org/Operations/Station_Architecture_Overview/Rivendell "Operations/Station_Architecture_Overview/Rivendell")
    -   [Signal Chain &
        Peripherals](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals")
        -   [Ballou
            Tower](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/Ballou_Tower "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/Ballou_Tower")
        -   [CD
            Players](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/CD_Players "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/CD_Players")
            -   [CDP-Denon](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/CD_Players/CDP-Denon "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/CD_Players/CDP-Denon")
            -   [CDR-Tascam](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/CD_Players/CDR-Tascam "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/CD_Players/CDR-Tascam")
        -   [Phones](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/Phones "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/Phones")
            -   [Patton 4118
                ATA](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/Phones/Patton_4118_ATA "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/Phones/Patton_4118_ATA")
            -   [Phone
                system](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/Phones/Phone_system "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/Phones/Phone_system")
        -   [StudioHub
            Peripherals](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/StudioHub_Peripherals "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/StudioHub_Peripherals")
            -   [CONP1](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/StudioHub_Peripherals/CONP1 "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/StudioHub_Peripherals/CONP1")
            -   [CONP2](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/StudioHub_Peripherals/CONP2 "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/StudioHub_Peripherals/CONP2")
            -   [CONSHP](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/StudioHub_Peripherals/CONSHP "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/StudioHub_Peripherals/CONSHP")
            -   [Fiber](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/StudioHub_Peripherals/Fiber "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/StudioHub_Peripherals/Fiber")
            -   [SASHP](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/StudioHub_Peripherals/SASHP "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/StudioHub_Peripherals/SASHP")
            -   [SAWJ](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/StudioHub_Peripherals/SAWJ "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/StudioHub_Peripherals/SAWJ")
            -   [SBWJ1](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/StudioHub_Peripherals/SBWJ1 "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/StudioHub_Peripherals/SBWJ1")
            -   [SBWJ2](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/StudioHub_Peripherals/SBWJ2 "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/StudioHub_Peripherals/SBWJ2")
            -   [SCSHP](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/StudioHub_Peripherals/SCSHP "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/StudioHub_Peripherals/SCSHP")
            -   [SCWJ](https://wiki.wmfo.org/index.php?title=Operations/Station_Architecture_Overview/Signal_Chain_%26_Peripherals/StudioHub_Peripherals/SCWJ "Operations/Station_Architecture_Overview/Signal_Chain_&_Peripherals/StudioHub_Peripherals/SCWJ")
-   [ToDo
    List](https://wiki.wmfo.org/Operations/Todo_List "Operations/Todo_List")

1.  1. [Contents](#Contents)

