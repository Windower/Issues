2013-08-06
----------
Attainment 2.2.5.6 - Arcon
* Fixed Abyssea and Dynamis trackng

2013-08-06
----------
InfoBar 1.1.0.4 - Arcon
* Fixed crash on load

2013-06-06
----------
Timers 1.0.1.12 - JoshK6656
* Fixed Merit values being used for time calculations.

LuaCore 1.5.0.8 - JoshK6656
* Fixed Merit table

2013-06-02
----------
Hook 4.0.0.35 - Iryoku
* Fixed bug with consecutive auto-translate phrases

Binder 1.4.0.1 - Iryoku
* Reenabled Razer BlackWidow 2013 Edition

2013-06-01
----------
Binder 1.4.0.0 - Iryoku
* Added Logitech G710+ Gaming Keyboard

ConsoleBG 2.3.0.8 - Arcon
* Added settings XML file to configure autoload settings

ConsoleBG 2.3.0.9 - Aureus
* Fixed white background on startup

Distance 1.3.1.5 - Arcon
* Added 3D mode options
* Added settings XML file

FFOChat 1.0.1.1 - Arcon
* Added &lt;showNames&gt; option to settings XML
* Fixed crash on closed TCP connection, added automatic reconnect

Hook 4.0.0.34 - Iryoku
* Fixed bug with add_to_chat()

LuaCore 1.0.5.5 - Arcon
* Added create_dir, file_exists and dir_exists functions
* Added engaged check to get_player()['in_combat']

LuaCore 1.0.5.6 - Arcon
* Fixed zoning LuaCore crash for get_player()['in_combar']

LuaCore 1.0.5.7 - Arcon
* Added lpack library for raw bit data manipulation
 * See addons/libs/packets.lua for example usage

PetTP 2.1.1.3 - Arcon
* Recompile against new Hook, minor internal changes

SpellCast 2.5.0.9 - Arcon
* Recompile against new Hook, no changes

TParty 1.2.0.7 - Arcon
* Target HP% position adjustment
* Various internal efficiency improvements
*
ConsoleBG 2.3.0.8 - Aureus
* Fixed issue where background would randomly decide to be white
* Settings XML should properly download now

2013-05-29
----------
Hook 4.0.0.33 - Aureus
* Refactoring, remove no longer used interfaces

LuaCore 1.0.5.4 - Aureus
* Add get_ability_recasts
 * http://dev.windower.net/doku.php?id=lua:interface_functions:input_functions:start#get_ability_recasts
* Add get_spell_recasts 
 * http://dev.windower.net/doku.php?id=lua:interface_functions:input_functions:start#get_spell_recasts

2013-05-24
----------
Timers 1.0.1.10 - Iryoku
* Added missing Blizzard II icon.

Timers 1.0.1.11 - Iryoku
* Fixed invalid buff durations for nonexistent buffs.

2013-05-22
----------
Launcher 4.0.4890.17383 - Iryoku
* Removed restrictions on registry value 0019: On-Screen Maps.

LuaCore 1.0.5.3 - Aureus
* Changed item extdata to start at index 1, not index 0, as per Lua convention.

2013-05-20
----------
LuaCore 1.0.5.2 - Aureus
* Configure garbage collector to run periodically and upon increased addon memory usage.

2013-08-25
----------
Launcher 4.0.4985.17832 - Iryoku
* Fixed parsing bug in `<gamma>`, `<uiscale>`, and `<supersampling>`.
