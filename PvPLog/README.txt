PvPLog 
Author:           Brad Morgan
Based on Work by: Josh Estelle, Daniel S. Reichenbach, Andrzej Gorski, Matthew Musgrove
Version:          3.2.1
Last Modified:    2010-12-21

README

Installation:
    You should have just downloaded PvPLog.zip
    This file will unzip to:
        PvPLog/
        PvPLog/README.txt
        PvPLog/CHANGES.txt
        PvPLog/TODO.txt
        PvPLog/PvPLog.toc       
        PvPLog/PvPLog.xml    
        PvPLog/PvPLog.lua       
        PvPLog/PvPLogButton.xml    
        PvPLog/PvPLogButton.lua       
        PvPLog/PvPLogUI.xml
        PvPLog/PvPLogUI.lua
        PvPLog/localization.lua
        PvPLog/MyMinimapButton.lua
        PvPLog/nopatch
        PvPLog2/PvPLog2.toc
        PvPLog2/nopatch

    Place the entire zip contents into your 
    <WoW>/Interface/AddOns directory.

    
Use:
    PvPLog will automatically log your PvP and duel wins and losses.

    You can enable/disable PvPLog with:
        /pvplog enable
        /pvplog disable
    When disabled PvPLog will *not* track any of your PvP activites.

    When you win/lose a PvP battle, or duel, PvPLog will notify you
    as the data is recorded.
    
    Whenever you mouseover someone for which you have a PvP record
    the mouseover tool tip will contain the number of wins and
    losses you have against that player (provided that option is enabled).
    It will also produce an audible ding on mouseover to inform you of
    a player you have a record with (if you have the ding sound enabled).
    At this time a message is also displayed overhead with your record
    (if you have the display enabled).

    When targetting a player you have a PvP record with, your record
    will be displayed below the target window.  This text is movable.
        /pvplog targetreset
            May be used to reset the text to its original position.

    You may enable or disable the floating text display.
        /pvplog display [enable|disable]

    You may enable or disable the ding sound.
        /pvplog ding [enable|disable]

    You may enable or disable the mouseover effects.
        /pvplog mouseover [enable|disable]

    You may disable all spam effects (mouseover, ding, floating
    display).
        /pvplog nospam

    You may open the configuration window that allows you to set
    most of the options.  
        /pvplog config
    This window can also be opened by right-clicking the PvPLog minimap
    button.  If you have Cosmos installed then a button will be added
    to the Earth Features Menu (or the Khaos menu if the Earth Features
    Menu is disabled) that will open and close the configuration window.
    If you have the myaddons addon installed then it will be added there
    as well.
    
    You may get some basic statistics using:
        /pvplog stats
        
    You may view your PvP stats in a window using:
        /pvplog pvp
        
    You may view your duel stats in a window using:
        /pvplog duel

    You may get the version of PvPLog with:
        /pvplog version

    You may get the vendor tag of PvPLog with:
        /pvplog vendor

    You may keep only the lastest N PurgeLogData records with:
        /pvplog keep <n>

    You may reset your PvPLog settings using:
        /pvplog reset confirm
    Be careful as this will erase all your records!
	
	The minimap button radius can be viewed with:
		/pl radius 
	The minimap button radius can be changed with:
		/pl radius <value>
	The minimap button position can be viewed with:
		/pl position
	The minimap button position can be changed with:
		/pl position <value>

    Debugging commands:
    
    Use of these commands could cause the permanent loss of accumulated
    data. Use at your own risk. These commands are english only.
    
        /pvplog debug [on|off]
            Turns debugging messages on or off. When debugging messages
            are on, they are sent to chat and to a per character array
            along with combat log messages.

        /pvplog debug perm
        Copies the debug flag to the per character saved variable array.

        /pvplog debug save
        Copies the array of debug/combat messages into another array.

        /pvplog debug clear
        Clears the array of debug/combat messages.

        /pvplog vars
            Send some internal variables to chat.

    /pvplog ignore [on|off]
        Turns the recording of targets to ignore on or off. Ignored
        targets provide a performance optimization and should be 
        left on (off provides some debugging with mobs).

        /pvplog pve [on|off]
        Turns debugging with hostile NPCs (mobs) on or off.
        (/pvplog ignore off required).

    /pvplog ignore clear
        Clears the ignore variables.

    /pvplog target clear
        Clears the target variables.

        /pvplog event1 [on|off]
        Turns event to chat debugging messages on or off.

        /pvplog event2 [on|off]
        Turns event to array debugging messages on or off.

        /pvplog combat [on|off]
        Turns combat to chat debugging messages on or off.

        /pvplog ui [on|off]
        Turns ui to chat debugging messages on or off.

        /pvplog ttm [on|off]
        Turns tooltip to chat debugging messages on or off.

        /pvplog ttv [on|off]
        Turns tooltip parsing debugging messages on or off.

        /pvplog ptc [on|off]
        Turns the recording of targets when PLAYER_TARGET_CHANGED on or off.

        /pvplog comm [on|off]
        Turns channel communication debugging messages on or off.

        /pvplog notify <channelname>
        Sends a test message to indicated channel (using PvPLogSendMessageOnChannel).

        /pvplog chat kill|death
        Sends a test message to the indicated channel (using PvPLogSendChatMessage).

        /pvplog chat self
        Sends a test message to the indicated channel (using PvPLogChatMsg).

    Updates for PvPLog are available from these AddOn sites:
    * http://www.wowroster.net

    Comments, questions, and suggestions can be made in the PvPLog forum
    at http://www.wowroster.net