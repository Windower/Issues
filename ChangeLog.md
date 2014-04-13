2014-04-13
----------

LuaCore 1.5.2.5 - Arcon
* Fixed not recognizing the `keyboard` event on autoload

2014-04-11
----------

Hook 4.2.1.8 - Arcon
* Possible fix for the random crashes to login screen

Timers 1.1.4.6 - Arcon
* Fixed Embolden bug and Stratagem display

LuaCore 1.5.2.4 - Arcon
* Yes, you did, but no one to blame but myself :<

2014-04-10
----------
LuaCore 1.5.2.3 - Nitrous
* Fixed the autorun/follow spam. And hopefully didn't break 1.5.2.2 fix because it wasn't committed >.>

LuaCore 1.5.2.2 - Arcon
* Fixed the `TellHistory` signature

LuaCore 1.5.2.1 - Arcon
* Fixed `windower.ffxi.get_info().chat_open`


2014-04-08
----------

Spellcast 2.6.2.14 - Arcon
* Fixed equipment related rules and variables

JaZero 1.2.2.6 - Arcon
* Fixed unlocking character movement on engage/disengage

LuaCore 1.5.2.0 - Arcon
* Added the following functions to `windower.ffxi`
  * [`windower.ffxi.run`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxirun)
  * [`windower.ffxi.toggle_walk`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxitoggle_walk_walk)
  * [`windower.ffxi.turn`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiturn_dir)

Itemizer 1.2.3.1 - Arcon
* Fixed storing/retrieving items to/from Mog Safe

Timers 1.1.4.5 - Arcon
* Fixed gear-augmented buffs

2014-04-07
----------

Hook 4.2.1.7 - Arcon
* Fixed crash on zoning

2014-04-05
----------

LuaCore 1.5.1.2 - Arcon
* Fixed follow/autorun-related values and functions

2014-04-02
----------

Hook 4.2.1.6 - Arcon
* Cleared temporary items on zoning

2014-04-01
----------

Hook 4.2.1.5 - Arcon
* Fixed temporary items not resetting on zone

Hook 4.2.1.4 - Arcon
* Fixed logging facilities

2014-03-31
----------

Find 1.0.5.1 - Arcon
* Added a `$USEDSPACE` token to Find

2014-03-29
----------

LuaCore 1.5.1.1 - Arcon
* Fixed crash when using map-related functions

GearCollector 1.0.4.4 - Arcon
* Adjusted to new Hook API, efficiency improvements

Itemizer 1.2.2.4 - Arcon
* Adjusted to new Hook API, efficiency improvements

Find 1.0.5.0 - Arcon
* Adjusted to new Hook API
* Minor recode, efficiency and stability improvements

2014-03-28
----------

LuaCore 1.5.1.0 - Arcon
* Adjusted to new Hook API

FFOChat 1.1.0.0 - Arcon
* Recode, added further customization options

Hook 4.2.1.3 - Arcon
* Amended packet-based data extraction
* Fixed certain item-related data extraction

2014-03-24
----------

WeatherMon 1.0.1.6 - Arcon
* Fixed correct sound playing

WeatherMon 1.0.1.5 - Arcon
* Fixed icon display

2014-03-23
----------

PetTP 2.2.0.5 - Arcon
* Fixed not displaying correctly

Hook 4.2.1.2 - Arcon
* Fixed item `extdata` field not populating correctly

2014-03-22
----------

LuaCore 1.5.0.10 - Arcon
* Added boolean bit packing to the `pack` library (identifier `q`)

Hook 4.2.1.1 - Arcon
* Moved job info to the packet-based extractor

2014-03-21
----------

ChatMon 1.10.0.3 - Arcon
* Fixed party invite, emote and examined events

2014-03-20
----------

LuaCore 1.5.0.9 - Arcon
* Added `count_<bag>` for all item bags in `windower.ffxi.get_items`
  * Returns the currently used amount of the respective inventory bag

2014-03-19
----------

Hook 4.2.1.0 - Arcon
* Fixed packet-based item data extraction

LuaCore 1.5.0.8 - Arcon
* Fixed `windower.get_camera`

PlasticSurgeon 1.1.1.5 - Arcon
* Fixed command handler

BlinkMeNot 3.1.0.3 - Cair
* Fixed unintended behavior during monstrosity and related activities.

PlasticSurgeon 1.1.1.4 - Cair
* Fixed unintended behavior during monstrosity and related activities.

AutoExec 2.8.1.4 - Arcon
* Fixed buff events

LuaCore 1.5.0.7 - Arcon
* Fixed buff events

Hook 4.2.0.5 - Arcon
* Adjusted inventory to backup from memory-based struct
  * This update will immediately fix related issues in other plugins such as Timers, Spellcast and LuaCore

2014-03-18
----------

WeatherMon 1.0.1.4 - Arcon
* Fixed crashing on load

Hook 4.2.0.4 - Arcon
* Fixed time-related structures
  * This update will immediately fix related issues in other plugins such as AutoExec and LuaCore

BlinkMeNot 3.1.0.2 - Arcon
* Fixed not loading correctly on initial login

Itemizer 1.2.2.4 - Arcon
* Fixed command handler

Spellcast 2.6.2.13 - Arcon
* Fixed status-based gear handling

Guildwork 1.4.2.3 - Arcon
* Fixed command handler

TParty 1.2.2.3 - Cair
* Fixed logout event and related issues

Timers 1.1.4.4 - Cair
* Fixed logout event and related issues

StatusTimer 1.2.2.7 - Cair
* Fixed logout event and related issues

Spellcast 2.6.2.12 - Cair
* Fixed logout event and related issues

Sandbox 1.0.1.4 - Cair
* Fixed logout event and related issues

LuaCore 1.5.0.6 - Cair
* Fixed logout event and related issues

GearCollector 1.0.4.3 - Cair
* Fixed logout event and related issues

InfoBar 1.2.0.5 - Cair
* Fixed logout event and related issues

Find 1.0.4.3 - Cair
* Fixed logout event and related issues

2014-03-17
----------

Attainment 2.2.6.5 - Arcon
* Adjusted to new Hook API

InfoBar 1.2.0.4 - Arcon
* Fixed crash on load

Spellcast 2.6.2.11 - Arcon
* Fixed earring/ring equipping and crashing issues

FFOChat 1.0.2.8 - Arcon
* Fixed not initializing properly on login

StatusTimer 1.2.2.6 - Arcon
* Adjusted to new Hook API

Find 1.0.4.2 - Arcon
* Adjusted to new Hook API

Itemizer 1.2.2.3 - Arcon
* Adjusted to new Hook API

Guildwork 1.4.2.2 - Arcon
* Adjusted to new Hook API

GearCollector 1.0.4.2 - Arcon
* Adjusted to new Hook API

Timers 1.1.4.3 - Arcon
* Adjusted to new Hook API

Spellcast 2.6.2.10 - Arcon
* Adjusted to new Hook API

LuaCore 1.5.0.5 - Arcon
* Adjusted to new Hook API

Hook 4.2.0.3 - Arcon
* Re-added item status to the item struct
* Fixed item slot calculation

Spellcast 2.6.2.9 - Arcon
* Fixed status values on autoset

FFOChat 1.0.2.7 - Arcon
* Fixed settings loading and chat output

Spellcast 2.6.2.8 - Cair
* Fixed gear swapping

AutoExec 2.8.1.3 - Arcon
* Fixed login event not executing

TParty 1.2.2.2 - Arcon
* Fixed target and party loading

Spellcast 2.6.2.7 - Arcon
* Fixed a crash when performing certain actions if the plugin was loaded before logging in

LuaCore 1.5.0.4 - Arcon
* Populated target information correctly

LuaCore 1.5.0.3 - Arcon
* Fixed a crash on login when using `windower.ffxi.get_player()` too quickly after login

ZoneTimer 1.2.1.4 - Arcon
* Adjusted to new Hook API

WinControl 1.6.1.4 - Arcon
* Adjusted to new Hook API

WeatherMon 1.0.1.3 - Arcon
* Adjusted to new Hook API

UpdateResources 1.0.1.4 - Arcon
* Adjusted to new Hook API

TParty 1.2.2.1 - Arcon
* Adjusted to new Hook API

Timestamp 2.2.1.3 - Arcon
* Adjusted to new Hook API

Timers 1.1.4.2 - Arcon
* Adjusted to new Hook API

Tickle 1.1.2.3 - Arcon
* Adjusted to new Hook API

Text 1.1.1.3 - Arcon
* Adjusted to new Hook API

StatusTimer 1.2.2.4 - Arcon
* Adjusted to new Hook API

SSOrganizer 1.5.1.3 - Arcon
* Adjusted to new Hook API

Silence 1.7.2.3 - Arcon
* Adjusted to new Hook API

Sandbox 1.0.1.2 - Arcon
* Adjusted to new Hook API

Run 1.3.1.3 - Arcon
* Adjusted to new Hook API

PlasticSurgeon 1.1.1.3 - Arcon
* Adjusted to new Hook API

PetTP 2.2.0.4 - Arcon
* Adjusted to new Hook API

Logger 1.5.1.4 - Arcon
* Adjusted to new Hook API

LightLuggage 3.3.2.3 - Arcon
* Adjusted to new Hook API

JaZero 1.2.2.5 - Arcon
* Adjusted to new Hook API

InfoBar 1.2.0.3 - Arcon
* Adjusted to new Hook API

IME 1.2.1.3 - Arcon
* Adjusted to new Hook API

Find 1.0.4.1 - Arcon
* Adjusted to new Hook API

FFOChat 1.0.2.6 - Arcon
* Fixed auto-joined channels not loading

FFOChat 1.0.2.5 - Arcon
* Adjusted to new Hook API

Distance 1.3.3.1 - Arcon
* Adjusted to new Hook API

Clock 2.4.1.3 - Arcon
* Adjusted to new Hook API

ChatMon 1.10.0.2 - Arcon
* Adjusted to new Hook API

ChatLink 1.0.1.3 - Arcon
* Adjusted to new Hook API

Cancel 1.0.1.4 - Arcon
* Adjusted to new Hook API

BoxHelper 1.3.1.4 - Arcon
* Adjusted to new Hook API

BlinkMeNot 3.1.0.1 - Arcon
* Adjusted to new Hook API

Binder 1.4.1.1 - Arcon
* Adjusted to new Hook API

AutoExec 2.8.1.2 - Arcon
* Adjusted to new Hook API

Itemizer 1.2.2.2 - Arcon
* Adjusted to new Hook API

2014-03-16
----------

Spellcast 2.6.2.6 - Arcon
* Adjusted to new Hook API

DrawDistance 2.2.1.3 - Arcon
* Adjusted to new Hook API

Bidder 1.4.1.6 - Arcon
* Adjusted to new Hook API

GearCollector 1.4.2.1 - Arcon
* Adjusted to new Hook API

ConsoleBG 2.3.2.1 - Arcon
* Adjusted to new Hook API

2014-03-15 - Windower 4.2 released
----------

LuaCore 1.5.0.2 - Arcon
* Adjusted to new Hook API

Hook 4.2.0.2 - Arcon
* Fixed a crash when determining the size of a certain struct

LuaCore 1.5.0.1 - Arcon
* Adjusted to new Hook API
* Fixed a crash on login with the new API, added safety-checks

Hook 4.2.0.1 - Arcon
* Changed the API slightly for a cleaner setup

LuaCore 1.5.0.0 - Arcon
* Adjusted to new Hook API
* Fixed one possible crash on unloading an addon
* Exposed current food, medicine and costume effect to the table returned by `windower.ffxi.get_player`
* Removed `linkshell_rank` from that same table (wasn't working right and it's easily determined if needed)

Hook 4.2.0.0 - Arcon
* Added data extraction from packets to Hook
* Consequences for plugins include:
  * No more memory-reliance and hence less chance of plugins breaking during updates
  * Items are no longer cleared when zoning, they are available to the API immediately after zoning
    * Note that this does not affect the in-game item display, only the Lua API
  * Allows us to reliably track stats that were impossible to accurately determine before (like food, medicine, weather, etc.)
  * Minor efficiency improvements as a lot of safety-checks could be removed

2014-03-12
----------

LuaCore 1.4.7.4 - Arcon
* Fixed one source of crashing during event registration

2014-03-09
----------

LuaCore 1.4.7.3 - Cair
* Adjusted table returned by `windower.ffxi.get_spell_recasts` to start with index 0 to match spell IDs

2014-03-08
----------

Guildwork 1.4.2.0 - Arcon
* Fixed crafting-related data collection
* Safe-guarded data-collection against injected and modified packets

2014-02-23
----------

LuaCore 1.4.7.2 - Arcon
* Changed the mob table returned by `windower.ffxi.get_mob_by_*`
  * Added `spawn_type`
  * Changed `model_size` to return `1` for regular sized models
* Text objects can now have negative values and will not wrap around the screen

AutoExec 2.8.1.1 - Arcon
* Fixed `examined` and `invite` events

LuaCore 1.4.7.1 - Nitrous
* Fixed available attachments and equipped frame.


2014-02-22
----------

LuaCore 1.4.7.0 - Arcon
* Added `menu_open` and `chat_open` to the `windower.ffxi.get_info` table
* `pack` module:
  * Changed `'b'` to `'c'` for unsigned char
  * Added `'b'` for bit values (only for unsigned numeric types)

2014-02-21
----------

LuaCore 1.4.6.3 - Arcon
* `pack` module:
  * Fixed fixed-size string unpacking

2015-02-19
----------

Attainment 2.2.6.4 - Arcon
* Adjusted for the update

2015-02-18
----------

Timers 1.1.4.0 - Arcon
* Adjusted for the update
* Adjusted settings parser

BlinkMeNot 3.1.0.0 - Arcon
* Internal adjustments/cleanup
* Adjusted for the update
* Adjusted settings parser

Spellcast 2.6.2.5 - Arcon
* Updated to new struct

LuaCore 1.4.6.2 - Arcon
* Updated to new struct
* Added dev function

PetTP 2.2.0.3 - Arcon
* Updated to new struct

PetTP 2.2.0.2 - Arcon
* Adjusted for the update
* Adjusted settings parser

FFXIDB 0.3.1.2 - Arcon, Cair
* Adjusted for the update
* Adjusted settings parser

JaZero 1.2.2.4 - Arcon, Cair
* Adjusted for the update

InfoBar 1.2.0.2 - Arcon, Cair
* Adjusted for the update

ConsoleBG 2.3.2.0 - Arcon
* Adjusted settings parser

LuaCore 1.4.6.1 - Cair
* Fixed `is_valid` attribute of mob tables

Find 1.0.4.0 - Arcon, JoshK6656
* Adjusted for the update
* Adjusted settings parser

2014-02-17 February FFXI update
----------

TParty 1.2.2.0 - Arcon
* Adjusted for the update

Distance 1.3.3.0 - Arcon
* Adjusted for the update
* Adjusted settings parser

GearCollector 1.0.4.0 - Arcon, JoshK6656
* Adjusted for the update
* Adjusted settings parser

Spellcast 2.6.2.4 - Arcon, JoshK6656
* Adjusted for the update
* Fixed elements for day and weather

LuaCore 1.4.6.0 - Arcon, JoshK6656
* Adjusted for the update
* Adjusted settings parser

Guildwork 1.4.1.4 - JoshK6656
* Adjusted for the update

2014-02-14
----------

FFXIDB 0.3.1.1 - Arcon
* Added `//ffxidb map save` option, which saves the current character's settings for all characters
* Fixed opacity settings (both reading from settings file and setting it with `//ffxidb map opacity <x>`)
* Internal signature fixes

2013-02-13
----------

LuaCore 1.4.5.0 - Arcon
* Fixed map-related commands (`windower.ffxi.get_position` and `windower.ffxi.get_map_data`)
* Internal signature fixes

2014-02-07
----------

FFXIDB 0.3.1.0 - Arcon
* Adjusted settings parsing
* Made all in-game commands save to the settings XML
* Fixed range-settings

2014-01-30
----------

Timers 1.1.3.1 - Arcon
* Fixed Barspell duration timers

Timers 1.1.3.0 - Arcon
* Fixed Timers display due to internal settings changes

2014-01-29
----------

Timers 1.1.2.1 - Nitrous
* Changed duration for barstatus/barelements to use the formula instead of static durations

Timers 1.1.2.0 - Nitrous
* Added Dynasty Gloves checks
* Added WHM Regen enhancement gear
* Changed settings to new API and added default values

2014-01-26
----------

FFXIDB 3.0.0.0 - Arcon
* Settings slightly renamed
* Will now save settings per character when the map is dragged/dropped and zoomed

2014-01-25
----------

LuaCore 1.4.4.5 - Arcon
* Fixed `windower.ffxi.get_mjob_data().available_frames` for PUP
  * `.available_attachments` is known to be bugged still

LuaCore 1.4.4.4 - Arcon
* Adjusted `windower.ffxi.get_mjob_data()` for PUP:
  * `.available_heads`, `.available_frames` and `.available_attachments` will now return a list of IDs

2014-01-24
----------

Hook 4.1.2.3 - Arcon
* Changed developer keys

Timers 1.1.1.5 - Arcon
* Fixed stratagem display

FFXIDB 0.2.3.0 - Arcon
* Fixed map display since update
* Fixed crash on startup with no target

2014-01-23
----------
BlinkMeNot 3.0.7.1 - Arcon
* Fixed character-specific settings loading on login

LuaCore 1.4.4.2 - Arcon
* Fixed stack corruption caused in outgoing text

2014-01-22
----------

LuaCore 1.4.4.1 - Iryoku
* Added argument to outgoing text indicating whether or not the text was injected

Hook 4.1.2.2 - Iryoku
* Added argument to outgoing text indicating whether or not the text was injected

Spellcast 2.6.2.3 - Arcon
* Fixed default group loading

LuaCore 1.4.4.0 - Arcon
* Fixed `windower.ffxi.get_info().day`
* Adjusted all resource values passed to be IDs instead of strings now

LuaCore 1.4.3.7 - Cair
* Fixed unregistering events

StatusTimer 1.2.2.3 - Cair
* Fixed incorrect timer displays

Spellcast 2.6.2.2 - Arcon
* Fixed job-related rules

2014-01-21
----------
InfoBar 1.2.0.1 - Arcon
* Fixed crash on login

Attainment 2.2.6.3 - Arcon
* Fixed crash on login

Spellcast 2.6.2.1 - Arcon
* Fixed file loading

Spellcast 2.6.2.0 - Cair
* Fixed multiple crashes

LuaCore 1.4.3.6 - Arcon
* Adjusted `windower.ffxi.get_player().buffs` to not show `0xFF` (no buff)

LuaCore 1.4.3.5 - Arcon
* Changed `windower.ffxi.get_info().zone` to proper capitalization

LuaCore 1.4.3.4 - Arcon
* Increased addon reload duration to 3 seconds after `//reload LuaCore`

Attainment 2.2.6.2 - Arcon
* Adjusted for new update

BlinkMeNot 3.0.7.0 - Arcon
* Fixed crash on login

LuaCore 1.4.3.3 - Arcon
* Fixed incorrect job level reporting in `windower.ffxi.get_player()` (for both `main_job` and `sub_job`)

LuaCore 1.4.3.2 - Arcon
* Adjusted `windower.ffxi.get_player().status` to return a string again

LuaCore 1.4.3.1 - Arcon
* Adjusted `windower.ffxi.get_info().zone` to return a string again

LuaCore 1.4.3.0 - Arcon
* Adjusted the `status change` event to return IDs again

2014-01-20 January FFXI update
----------

Itemizer 1.2.2.0 - Cair
* Fixed for new Inventory struct

GearCollector 1.0.3.0 - Cair
* Fixed for new Inventory struct

Find 1.0.3.0 - Cair
* Fixed for new Inventory struct

FFXIDB 0.2.2.0 - Cair
* Fixed for new Party struct

BoxHelper 1.3.1.3 - JoshK6656
* Fixed for new Party struct

TParty 1.2.1.3 - JoshK6656
* Fixed for new Party struct

BlinkMeNot 3.0.6.9 - JoshK6656
* Fixed for new Party struct

Timers 1.1.1.4 - JoshK6656
* Fixed for new Inventory struct

StatusTimer 1.2.2.2 - JoshK6656
* Fixed for new Inventory struct

2014-01-12
----------
LuaCore 1.4.2.4 - Arcon
* Added `CondenseError` option in LuaCore's settings XML
  * Setting it to `true` will shorten the file path to the beginning of the addons folder
  * Setting it to `false` (default) will display the full file path

2014-01-11
----------
LuaCore 1.4.2.3 - Arcon
* Added `ErrorNewLine` option in LuaCore's settings XML
  * Setting it to `true` will insert newlines before the error message, to avoid the text going outside of the screen
  * Setting it to `false` (default) will make them display in one line as they were until now

ChatMon 1.10.0.1 - Arcon
* Fixed the party invite event

2014-01-07
----------
LuaCore 1.4.2.2 - Arcon
* Renamed the merit values `hp` and `mp` back to `max_hp` and `max_mp`

LuaCore 1.4.2.1 - Arcon
* Fixed merit typos
* Renamed the merit values `max_hp` and `max_mp` to `hp` and `mp`

Timers 1.1.1.2 - Nitrous
* Added Atrophy Gloves/+1 check
* Fixed Saber Dance check so that it actually checks for buff

2014-01-06
----------
LuaCore 1.4.2.0 - Cair
* Changed event registration handling to allow registration in asynchronous events and facilitate registration and removal in user environments
* Removed `time_string` from `windower.ffxi.get_info`
* Changed `get_mob_by_target` to use `<t>` if no argument is provided

Timers 1.1.1.1 - Nitrous
* Fixed extremely long timers for category 14 items that aren't sambas.

LuaCore 1.4.1.5 - Arcon
* Fixed crashing bug with `windower.ffxi.get_position`

LuaCore 1.4.1.4 - Arcon
* Added `get_position` and `get_map_data` to `windower.ffxi`
  * `get_position` returns the position string (same as `<pos>`)
  * `get_map_data` returns the internally used map ID as well as the pixel coordinates
  * For full documentation, see the wiki entry for [`get_position`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiget_position_index_x_y_z) and [`get_map_data`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiget_map_data_index_x_y_z)

2014-01-05
----------
GearCollector 1.0.2.4 - Nitrous
* Rebuilt for new api
* Made furnishings exempt from collection/putting away

LuaCore 1.4.1.3 - Nitrous
* Fixed `windwer.ffxi.get_mob_by_target` for `<r>` and `<bt>`

LuaCore 1.4.1.2 - Arcon
* Made `windower.ffxi.get_player().treasure` start at `0` to match the internal ID

LuaCore 1.4.1.1 - Arcon
* Adjusted inaccurate error message and removed erroneous safety check

LuaCore 1.4.1.0 - Arcon
* Fixed lotting/passing with packets
* Made `windower.ffxi.lot_item` and `windower.ffxi.pass_item` go off the internal memory ID, since that is also used in packets
* Changed `windower.ffxi.get_player().treasure` to also show items ordered by their internal ID to match the lot/pass changes

2014-01-04
----------
FFXIDB 0.2.1.7 - Nitrous
* Fix - Mouse Dragging

FFXIDB 0.2.1.6 - Nitrous
* Fix - Dots werent showing for players/monsters
* Added feedback when toggling display of dots and targetlines

Timers 1.1.1.0 - Nitrous
* Added Samba duration timers + gear extensions
* Fixed Circle Duration and added gear extensions
* Rebuilt for new API 

2014-01-03
----------
LightLuggage 4.0.1.0 - Arcon
* Re-enabled auto-stacking

LightLuggage 4.0.0.0 - Arcon
* Recoded completely except for the file parsing
* Stopped spamming packets when not necessary
* Won't auto-sort inventory anymore except on login
  * There is now an in-game option to keep the inventory sorted

2014-01-02
----------
Distance 1.3.2.4 - Nitrous
* Rebuilt against new API

Hook 4.1.2.1 - Arcon
* Added Nitrous's development key

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

