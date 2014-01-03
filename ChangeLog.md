2014-01-02
----------
Spellcast 2.6.1.0 - Arcon
* Fixed the permanent autoset triggering
* Fixed accessing targets by party specifier (`<p0>`, `<p1>`, etc.)

LuaCore 1.4.0.6 - Cair
* Fixed outgoing packet functions for blue magic and puppetmaster.

Spellcast 2.6.0.13 - Cair
* Fixed player status assignment on initial login

LuaCore 1.4.0.5 - Cair
* Fixed player status assignment on initial login

FFXIDB 0.2.1.5 - Arcon
* Fixed map looping when zooming out too far

Spellcast 2.6.0.12 - Arcon
* Fixed `(regex)` formatted rules
* Fixed another access violation in the `OutgoingText` method

AutoExec 2.8.0.3 - Arcon
* Fixed `(regex)` formatted events

2014-01-01
----------
Spellcast 2.6.0.11 - Cair
* Fixed `<st*>` handling

LuaCore 1.4.0.4 - Arcon
* Added `windower.execute`.
  * See the [wiki entry](http://dev.windower.net/doku.php?id=lua:api:functions:start&#windowerexecute_file_arguments) for documentation

Launcher 4.1.5114.38760 - Arcon
* Made the `-u|--update` option launch the program invisibly

Spellcast 2.6.0.10 - Cair
* Fixed the access violation in the `OutgoingText` method

Spellcast 2.6.0.9 - Cair
* Fixed target rules

LuaCore 1.4.0.3 - Cair
* Removed unused `target` from `ffxi.get_info`
* Fixed moon phase

Launcher 4.1.5114.21982 - Arcon
* Added `-u|--update` option to only update files then immediately close without launching POL

AutoExec 2.8.0.2 - Arcon
* Rebuilt against new API to fix certain events

Spellcast 2.6.0.8 - Arcon
* Fixed targeting issues

LuaCore 1.4.0.2 - Arcon
* Re-added `nil` returns on invalid event registry (stable)

2013-12-31
----------
LuaCore 1.4.0.1 - Cair
* Temporarily fixed crashing on invalid event registry

Spellcast 2.6.0.7 - Cair
* Fixed expression parsing

Spellcast 2.6.0.6 - Cair
* Re-implemented autodetection of party member names

PetTP 2.2.0.1 - Cair
* Recompiled to handle invalid mob array

Spellcast 2.6.0.5 - Arcon
* Adjusted for the fixed job change event

LuaCore 1.4.0.0 - Arcon
* Adjusted the Lua parser to allow indexing and calling of literals

LuaCore 1.3.0.9 - Cair
* Added `valid_target` to the mob table

LuaCore 1.3.0.8 - Arcon
* Amended the Lua parser to accept the unary plus (including metamethod `__unp`)

LuaCore 1.3.0.7 - Cair
* Fixed job change event
* Added `lot_item` and `pass_item` to `windower.ffxi`
  * See the [wiki entry](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start#windowerffxilot_item_slot) for documentation

LuaCore 1.3.0.6 - Arcon
* Fixed party struct

2013-12-30
----------
Timers 1.1.0.1 - Arcon
* Added *Flee* enhancing items

LuaCore 1.3.0.5 - Arcon
* Fixed time-related functions and variables

Spellcast 2.6.0.4 - Arcon
* Fixed time-related functions and variables

2013-12-29
----------
LuaCore 1.3.0.4 - Arcon
* Fixed bracket enclosed (`<*>`) value support in `windower.ffxi.get_mob_by_target`

LuaCore 1.3.0.3 - Arcon
* Fixed setting character info before triggering the login event

LuaCore 1.3.0.2 - Arcon
* Fixed junk ID byte on certain packet-related functions

2013-12-28
----------
AutoExec 2.8.0.1 - Cair
* Adjusted for auto-translated text in events

LuaCore 1.3.0.1 - Cair
* Adjusted for auto-translated text in events

Timers 1.1.0.0 - Arcon
* Major internal API revamp

Chatmon 1.10.0.0 - Arcon
* Major internal API revamp

AutoExec 2.8.0.0 - Arcon
* Major internal API revamp

LuaCore 1.3.0.0 - Arcon
* Major internal API revamp

Spellcast 2.6.0.0 - Arcon
* Major internal API revamp

StatusTimer 1.2.2.1 - JoshK6656
* Added support for all Lv.119 mythic weapon types

2013-12-27
----------
LuaCore 1.2.2.1 - Cair
* Added boolean values `charmed`,`in_party`, and `in_alliance` to `windower.ffxi.get_mob_by_*` functions

2013-12-25
----------
StatusTimer 1.2.2.0 - JoshK6656
* Added Lv.119 mythic support

AutoExec 2.7.10.8 - Cair
* Recompiled against new API to fix an issue with new zones

LightLuggage 3.3.2.3 - Cair
* Recompiled against new packet API to stop sending bad packets

2013-12-24
----------
LuaCore 1.2.2.0 - Arcon
* Rewrote packet injecting mechanics, fixed deadlock

2013-12-23
----------
Timers 1.0.2.9 - Cair
* Fixed job change to appropriately clear current timers. 

LuaCore 1.2.1.12 - Arcon
* Fixed crash on zoning with certain addons loaded

LuaCore 1.2.1.11 - Arcon
* Fixed `windower.ffxi.get_mob_by_target('st')`
* Added `last_incoming` and `last_outgoing` to `windower.packets`
  * See the [wiki entry](http://dev.windower.net/doku.php?id=lua:api:functions:packets:start&#windowerpacketslast_incoming_id) for documentation

2013-12-22
----------
Hook 4.1.2.0 - Arcon
* Added removal of duplicate packets based on a whitelist
  * If you want us to add more packets to the whitelist, let us know
* Made injected packets trigger `(incoming|outgoing) chunk` events

LuaCore 1.2.1.10 - Arcon
* Added `nil` return to `windower.ffxi.get_mob_by_*` functions

LuaCore 1.2.1.9 - Arcon
* Fixed crashes when trying to access the mob array when logged out

2013-12-21
----------
LuaCore 1.2.1.8 - Arcon
* Changed the `time change` event to return the number of minutes
* Fixed the various `linkshell` values in `windower.ffxi.get_player()`
  * **Note:** Only takes effect after zoning or changing it once, will need to be adjusted

2013-12-19
----------
LuaCore 1.2.1.7 - Arcon
* Added boolean `autorun` value to `windower.ffxi.get_player()`

LuaCore 1.2.1.6 - Arcon
* Partially fixed events that take string arguments

LuaCore 1.2.1.5 - Cair
* Fixed crash when using `windower.ffxi.get_mob_by_target` while logged out

2013-12-18
----------
LuaCore 1.2.1.4 - Arcon
* Fixed "file does not exist" error on `lua exec`

2013-12-17
----------
Infobar 1.1.1.5 - Arcon
* Fixed crash on logout

2013-12-15 - Windower 4.1 released
----------
Hook 4.1.1.4 - Group effort
* New text renderer
* New console display and console options
  * `console_color [alpha] <red> <green> <blue>`
  * `console_font <name> [size]`
  * `console_timestamp [0|1]`
* Added mouse and keyboard events to the plugin API
* Minor controller bug fix for multiboxing

LuaCore 1.2.1.3 - Group effort
* Revamped entire API, multiple additions, some removals
  * See [API documentation](http://dev.windower.net/doku.php?id=lua:api:start)
* Changed addons to run on their own threads
* Changed event scheduling
  * `windower.register_event('event name', function_to_execute)`
* `_addon` table now exists by default, can take the following values:
  * _String_ `name`
  * _String_ `author`
  * _String_ `language`
  * _String_ `version`
  * _String_ `command`
  * _Table_ `commands`

FFXIDB 0.2.1.4 - Zohno
* Added draggable/scrollable minimap

All plugins - Group effort
* Updated to match the new API and various minor fixes

2013-12-02
----------
Spellcast 2.5.0.18 - Cairthenn
* Fixed auto-translated command issue

2013-11-30
----------
Attainment 2.2.5.8 - Arcon
* Fixed version mismatch

Timers 1.0.1.16 - Cairthenn
* Various equipment related fixes (Carnwenhan, Brioso Slippers/Roundlet, Legato Dagger)

2013-11-29
----------
Attainment 2.2.5.7 - Arcon
* Fixed Abyssea lights since last update

2013-10-12
----------
GearCollector 1.0.1.0 - Aureus
* Moved storage priority up, items are now being checked in the following order:
  * Safe > Locker > Storage > Satchel > Sack > Case

2013-10-07 - 2013-10-12
----------
Various updates happened in this time frame, most very fast paced and bug fixes of previous releases to adjust for the Mog Case and changes to the inventory struct due to it. The following is a listing of the final releases.

Find 1.0.1.4 - JoshK6656
* Adjusted for new inventory struct

GearCollector 1.0.0.9 - JoshK6656
* Adjusted for new inventory struct

Guildwork 1.3.2.0 - JoshK6656
* Adjusted for new inventory struct

Itemizer 1.2.0.5 - JoshK6656
* Adjusted for new inventory struct

LuaCore 1.0.6.4 - JoshK6656
* Adjusted for new inventory struct

Timers 1.0.1.15 - JoshK6656
* Adjusted for new inventory struct

Blinkmenot 3.0.5.3 - JoshK6656
* Adjusted for new inventory struct and adjusted combat check

Spellcast 2.5.0.14 - JoshK6656
* Adjusted for new inventory struct and adjusted combat check

2013-08-25
----------
Launcher 4.0.4985.17832 - Iryoku
* Fixed parsing bug in `<gamma>`, `<uiscale>`, and `<supersampling>`.

2013-08-06
----------
Attainment 2.2.5.6 - Arcon
* Fixed Abyssea and Dynamis tracking

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
* Reenabled *Razer BlackWidow 2013* Edition

2013-06-01
----------
Binder 1.4.0.0 - Iryoku
* Added *Logitech G710+* Gaming Keyboard

ConsoleBG 2.3.0.8 - Arcon
* Added settings XML file to configure autoload settings

ConsoleBG 2.3.0.9 - Aureus
* Fixed white background on startup

Distance 1.3.1.5 - Arcon
* Added 3D mode options
* Added settings XML file

FFOChat 1.0.1.1 - Arcon
* Added `<showNames>` option to settings XML
* Fixed crash on closed TCP connection, added automatic reconnect

Hook 4.0.0.34 - Iryoku
* Fixed bug with `windower.add_to_chat`

LuaCore 1.0.5.5 - Arcon
* Added `windower.create_dir`, `windower.file_exists` and `windower.dir_exists` functions
* Added engaged check to `windower.ffxi.get_player().in_combat`

LuaCore 1.0.5.6 - Arcon
* Fixed zoning LuaCore crash for `windower.ffxi.get_player().in_combat`

LuaCore 1.0.5.7 - Arcon
* Added *lpack* library for raw bit data manipulation
 * See `Windower/addons/libs/packets.lua` for example usage

PetTP 2.1.1.3 - Arcon
* Recompile against new Hook, minor internal changes

SpellCast 2.5.0.9 - Arcon
* Recompile against new Hook, no changes

TParty 1.2.0.7 - Arcon
* Target HP% position adjustment
* Various internal efficiency improvements

ConsoleBG 2.3.0.8 - Aureus
* Fixed issue where background would randomly decide to be white
* Settings XML should properly download now

2013-05-29
----------
Hook 4.0.0.33 - Aureus
* Refactoring, remove no longer used interfaces

LuaCore 1.0.5.4 - Aureus
* Add `windower.ffxi.get_ability_recasts`
 * http://dev.windower.net/doku.php?id=lua:interface_functions:input_functions:start#get_ability_recasts
* Add `windower.ffxi.get_spell_recasts`
 * http://dev.windower.net/doku.php?id=lua:interface_functions:input_functions:start#get_spell_recasts

2013-05-24
----------
Timers 1.0.1.10 - Iryoku
* Added missing *Blizzard II* icon.

Timers 1.0.1.11 - Iryoku
* Fixed invalid buff durations for nonexistent buffs.

2013-05-22
----------
Launcher 4.0.4890.17383 - Iryoku
* Removed restrictions on registry value `0019`: *On-Screen Maps*.

LuaCore 1.0.5.3 - Aureus
* Changed item extdata to start at index 1, not index 0, as per Lua convention.

2013-05-20
----------
LuaCore 1.0.5.2 - Aureus
* Configure garbage collector to run periodically and upon increased addon memory usage.

