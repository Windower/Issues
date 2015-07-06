2015-07-06
----------

JaZero 1.2.2.13 - Arcon
* Fixed the engage/disengage unlock not working

2015-06-27
----------

BlinkMeNot 3.1.0.10 - Arcon
* Fixed for update
* Fixed target handling

Guildwork 1.4.2.9 - Arcon
* Fixed for update
* Fixed target handling

2015-06-27
----------

FFXIDB 0.9.2.7 - Arcon
* Fixed target handling
* Adjusted the target line to show the sub-target, when available

InfoBar 1.2.0.13 - Arcon
* Fixed target handling

LuaCore 2.0.1.6 - Arcon
* Fixed target handling

2015-06-26 June FFXI Update
----------

FFXIDB 0.9.2.6 - Arcon
* Fixed for update

Timers 3.7.4.3 - Arcon
* Fixed for update

LuaCore 2.0.1.5 - Arcon
* Fixed for update

2015-05-25
----------

Blinkmenot 3.1.0.9 - Byrth
* Recompiled per Arcon's request

Timers 3.7.4.2 - Byrth
* Recompiled per Arcon's request

2015-05-24
----------

LuaCore 2.0.1.4 - Byrth
* Adjusted `windower.ffxi.get_abilities().job_abilities` so it is no longer limited to 752 abilities
* Added the new job point categories to `windower.ffxi.get_player().job_points`

2015-05-18
----------

InfoBar 1.2.0.12 - Arcon
* Fixed NPC related info

FFXIDB 0.9.2.5 - Arcon
* Fixed NPC display

LuaCore 2.0.1.3 - Arcon
* Fixed `windower.ffxi.get_mob_by_target('lastst')`

2015-05-15 May FFXI Update
----------

LuaCore 2.0.1.2 - Arcon
* Added `equipment` as a possible parameter to `windower.ffxi.get_items`

LuaCore 2.0.1.1 - Arcon
* Fixed inventory even more
* Added `safe2` as a key to the `windower.ffxi.get_items` table, and enabled it as a function parameter
* Added `max_safe2`, `count_safe2` and `enabled_safe2` values to the `windower.ffxi.get_items` table
* Added `max_safe2`, `count_safe2` and `enabled_safe2` values to the `windower.ffxi.get_bag_info` table
* Fixed pet and fellow related variables

LuaCore 2.0.1.0 - Arcon
* Fixed inventory
* Adjusted `windower.ffxi.get_items` to accept all its table keys as function parameters
  * `inventory`
  * `safe`
  * `storage`
  * `temporary`
  * `locker`
  * `satchel`
  * `sack`
  * `case`
  * `wardrobe`
  * `safe2`
  * `treasure`
  * `gil`

Hook 4.2.12.4 - Iryoku
* Fixed inventory and related bugs

2015-05-06
----------

LuaCore 2.0.0.0 - Arcon
* Added support for the *SQLite* database, provided by the [LuaSQLite3](http://lua.sqlite.org/index.cgi/home) library

2015-04-05
----------

Timers 3.7.4.1 - Byrth
* Added *Phantom Roll* upgrades from reforged COR Empyrean armor

LuaCore 1.9.2.4 - Arcon
* Added `server` ID to the table returned by `windower.get_info`

Config 2.0.0.3 - Arcon
* Fixed crash on logout

2015-04-04
----------

Hook 4.2.12.3 - Arcon
* Adjusted developer keys

2015-04-01
----------

Hook 4.2.12.2 - Arcon
* Fixed pasting not working immediately after opening the chat input box
* Fixed the `%` modifier occasionally ignoring an open chat input box

LuaCore 1.9.2.3 - Arcon
* Fixed erroneous prevention of setting *Blue Magic* spells

Timers 3.7.4.0 - Byrth, Arcon
* Added March 2015 update items
* Fixed enhancing duration buffs from *Ghostfyre Cape* and various augments

2015-03-27
----------

FFXIDB 0.9.2.4 - Arcon
* Fixed an issue where targeting could cause crashes
* Fixed an issue where target lines were not displayed correctly

Launcher 4.2.5564.39846 - Arcon
* Fixed an issue where FFXI would not start up

Launcher 4.2.5564.39373 - Arcon
* Fixed an issue where the Launcher would not start up on certain operating systems

LuaCore 1.9.2.2 - Arcon
* Fixed `windower.ffxi.get_mob_by_target('lastst')`

2015-03-26 March FFXI Update
----------

JaZero 1.2.2.12 - Arcon
* Fixed for March update

LuaCore 1.9.2.1 - Arcon
* Fixed `windower.ffxi.get_mob_by_target` being broken for certain values

LuaCore 1.9.2.0 - Arcon
* Fixed crash in `windower.ffxi.get_ability_recasts`
* Adjusted `windower.regex.match` to return tables for sub-groups

2015-03-21
----------

Launcher 4.2.5558.22522 - Arcon
* Fixed an issue where the addons are not updated correctly for Windows XP users
  * Addons will still not be updated in real time, so delays between addon pushes and updates for Windows XP users are expected

2015-03-16
----------

Launcher 4.2.5553.33791 - Arcon
* Fixed an issue where the Launcher would not start under certain conditions

2015-03-15
----------

Launcher 4.2.5552.23154 - Arcon
* Fixed an issue where addons and plugins would not correctly load in the dev version

Launcher 4.2.5552.21628 - Arcon
* Added a `--quit` option which quits the *Launcher* before the *PlayOnline Viewer* starts
  * This is only useful to update *Windower* silently
* Re-added the `--update` option which makes implies both `--hide` and `--quit`

2015-03-14
----------

Launcher 4.2.5551.19172 - Arcon
* Changed the `--update` option to `--hide` due to a misleading name

2015-03-08
----------

StatusTimer 1.2.3.0 - Byrth
* Fixed *Aftermath* calculations
* Added *Aftermath* calculations for *Ergon* weapons

2015-02-26
----------

LuaCore 1.9.1.2 - Arcon
* Fixed `windower.ffxi.get_mjob_data` and `windower.ffxi.get_sjob_data` reporting incorrect BLU spells

2015-02-25
----------

Timers 3.7.3.0 - Arcon
* Added optional third argument when creating custom timers that indicates whether the bar is moving up or down
  * `timers c <name> <duration> [up|down]`

InfoBar 1.2.0.11 - Arcon
* Fixed the crash when trying to display current player information

LuaCore 1.9.1.1 - Arcon
* Fixed contents of the tables returned by `windower.ffxi.get_mjob_data` and `windower.ffxi.get_sjob_data`

Hook 4.2.12.1 - Arcon
* Fixed gathered data regarding job info

2015-02-20
----------

FFXIDB 0.9.2.3 - Arcon
* Adjusted for February FFXI update

LuaCore 1.9.1.0 - JoshK6656
* Added new Job Points to the Lua API

2015-02-19 February FFXI Update
----------

LuaCore 1.9.0.5 - Arcon
* Fixed incorrect job ability recasts being reported with `windower.ffxi.get_ability_recasts`

LuaCore 1.9.0.4 - Arcon
* Fixed incorrect error message output under certain circumstances

InfoBar 1.2.0.10 - Arcon
* Adjusted for February FFXI update

BlinkMeNot 3.1.0.8 - Arcon
* Adjusted for February FFXI update

JaZero 1.2.2.11 - Arcon
* Adjusted for February FFXI update

Timers 3.7.2.0 - Arcon
* Adjusted for February FFXI update
* Added *Grapevine Cape*'s bonus to *Battery Charge*
* Fixed *Killer Instinct* duration calculations based on additional merit points

LuaCore 1.9.0.3 - Arcon
* Adjusted for February FFXI update

2015-02-18
----------

LuaCore 1.9.0.2 - Arcon
* Fixed the bug that caused `lua list` to print to the console and `lua list console` to print to the chat log

LuaCore 1.9.0.1 - Arcon
* Fixed a bug in the `windower.send_command` function that would cause a crash with certain inputs

LuaCore 1.9.0.0 - Cair
* Added the [`windower.pipe`](http://dev.windower.net/doku.php?id=lua:api:functions:pipe:start) table with functions allowing communication with programs over named pipes.
  * This functionality is in development and subject to heavy API changes.
* Added the `pipe message` event that triggers when a message is received over the named pipe.
  * This functionality is in development and subject to heavy API changes.


2015-02-15
----------

LuaCore 1.8.6.1 - Arcon
* Fixed error reporting
  * All syntax errors were incorrectly reported as "attempt to call a string value"

Timers 3.7.1.2 - Arcon
* Added the *Ghostfyre Cape* to *Enhancing Magic* duration calculations

Config 2.0.0.2 - Arcon
* Fixed an issue where the `AutoDisconnect` option would be reset to the game's default after zoning

2015-02-14
----------

LuaCore 1.8.6.0 - Arcon
* Added the [`windower.chat`](http://dev.windower.net/doku.php?id=lua:api:functions:chat:start) table with functions relating to chat input

Hook 4.2.12.0 - Arcon
* Fixed a number of old pasting-related crashes and chat corruption
  * Game won't crash when browsing the chat history after pasting anymore
  * Game won't crash when removing pasted text a number of times anymore
  * Pasting won't mess up auto-translate phrases anymore
* Some minor stability adjustments

2015-02-11
----------

LuaCore 1.8.5.0 - Arcon
* Changed the default behavior of `//lua list`
  * Will now output to the chat log by default
  * If provided the optional keyword `console` will output to the Windower console as it did before
* Added an optional argument to `//lua memory` which will only show the memory usage of addons starting with the provided string

LuaCore 1.8.4.0 - Arcon
* Added [`windower.get_from_clipboard`](http://dev.windower.net/doku.php?id=lua:api:functions:start&#windowerget_from_clipboard) and [`windower.copy_to_clipboard`](http://dev.windower.net/doku.php?id=lua:api:functions:start&#windowercopy_to_clipboard_str) functions to the Lua API

2015-02-1
----------

Timers 3.7.1.1 - Arcon
* Fixed certain *Scholar* buffs not wearing off correctly

2015-01-31
----------

Config 2.0.0.1 - Arcon
* Changed the default `FrameRateDivisor` option from 1 to 2
  * That means that the default frame rate cap was changed to 30 FPS (the game's native limit)

Config 2.0.0.0 - Arcon
* Revamped the settings handler
* Added `config help` option to display all possible settings
* Merged `MapDrawDistance` and `MobDrawDistance` into the `ClippingPlane` option
  * Both single options are still available and will take precedence over `ClippingPlane`
  * They merely won't be necessary anymore and can be omitted to only have one value
* Added `AutoDisconnectTime` option
  * If set to a number bigger than 0 it will enable the game's auto-disconnect feature
* Fixed aspect ratio resetting on zoning
  * Will now completely disable the game's own slider

2015-01-26
----------

Timers 3.7.1.0 - Arcon
* Improved buff handling of certain buffs
  * This change fixed certain Scholar-related buff timers incorrectly staying after wearing off
  * Afftected buffs were:
    * *Light Arts*
    * *Dark Arts*
    * *Sublimation*
    * *Stratagems*
* Fixed composure incorrectly multiplying the buff duration by 2 instead of 3

2015-01-18
----------

Config 1.1.0.2 - Arcon
* Fixed incorrect aspect ratio calculation for explicitly provided values

Config 1.1.0.1 - Arcon
* Fixed incorrect settings names

2015-01-17
----------

Config 1.1.0.0 - Arcon
* Incorporated Unlimited's functionality
  * The game divides 60 FPS by the value `FrameRateDivisor` to determine the frame rate cap
  * The default is `2`, resulting in a 30 FPS cap
  * Set it to `1` to increase the cap to 60 FPS
  * Setting it to `0` will disable the cap entirely, but will likely cause performance problems

2015-01-16
----------

Config 1.0.1.0 - Arcon
* Added `save` command to save the current character's settings globally

2015-01-15 January FFXI Update
----------

Hook 4.2.11.5 - Arcon
* Fixed chat related issues

GearCollector 1.0.4.7 - Arcon
* Adjusted to new API

Guildwork 1.4.2.8 - Arcon
* Adjusted to new API

WinControl 1.6.1.5 - Arcon
* Adjusted to new API

WeatherMon 1.0.1.9 - Arcon
* Adjusted to new API

Tickle 1.1.2.4 - Arcon
* Adjusted to new API

StatusTimer 1.2.2.9 - Arcon
* Adjusted to new API

SSOrganizer 1.5.1.7 - Arcon
* Adjusted to new API

Run 1.3.1.4 - Arcon
* Adjusted to new API

PlasticSurgeon 1.1.1.6 - Arcon
* Adjusted to new API

Logger 1.5.1.5 - Arcon
* Adjusted to new API

LightLuggage 4.0.1.2 - Arcon
* Adjusted to new API

InfoBar 1.2.0.9 - Arcon
* Adjusted to new API

IME 1.2.1.5 - Arcon
* Adjusted to new API

DelayMeNot 1.0.0.2 - Arcon
* Adjusted to new API

ChatMon 1.10.0.4 - Arcon
* Adjusted to new API

BlinkMeNot 3.1.0.7 - Arcon
* Adjusted to new API

Bidder 1.4.1.9 - Arcon
* Adjusted to new API

AutoExec 2.8.1.7 - Arcon
* Adjusted to new API

Unlimited 1.0.1.1 - Arcon
* Adjusted to new API

Timers 3.7.0.3 - Arcon
* Adjusted to new API

Sandbox 1.0.1.6 - Arcon
* Adjusted to new API

JaZero 1.2.2.10 - Arcon
* Adjusted to new API

FishingCrashFix 1.0.0.1 - Arcon
* Adjusted to new API

FFXIDB 0.9.2.2 - Arcon
* Adjusted to new API

FFOChat 1.1.1.1 - Arcon
* Adjusted to new API

Config 1.0.0.1 - Arcon
* Adjusted to new API

Binder 1.4.2.0 - Arcon
* Adjusted to new API
* Added ASUS Strix Tactic Pro
* Added Logitech ChillStream

LuaCore 1.8.3.3 - Arcon
* Adjusted to new API

LuaCore 1.8.3.2 - Arcon
* Fixed incoming chunk crash when receiving messages

Hook 4.2.11.4 - Arcon
* Fixed auto-translating signature

2015-01-14
----------

Hook 4.2.11.3 - Arcon
* Fixed an error that would cause texts and prims to be removed immediately after creation in certain instances

LuaCore 1.8.3.1 - Arcon
* Fixed a bug in `windower.prim.get_position`

LuaCore 1.8.3.0 - Arcon
* Added the [`windower.console`](http://dev.windower.net/doku.php?id=lua:api:functions:console:start) table to the Lua API along with the respective functions

2015-01-09
----------

Timers 3.7.0.2 - Arcon
* Fixed an error where recast names of abilities would display incorrectly

Timers 3.7.0.1 - Arcon
* Fixed shared timer names not displaying properly

2015-01-08
----------

Timers 3.7.0.0 - Arcon
* Replaced the old `recastList` and `buffsList` options with more detailed equivalents
  * `AbilityRecastFilter`
  * `AbilityBuffFilter`
  * `SpellRecastFilter`
  * `SpellBuffFilter`
* Fixed a bug where the `recastList` and `buffsList` settings were ignored
* Adjusted *Timers* to delete unused settings values
 * The settings have been updated quite a few times, resulting in many unused values cluttering up the XML files

FFOChat 1.1.1.0 - Arcon
* Added full Shift JIS input support

2015-01-07
----------

LuaCore 1.8.2.0 - Arcon
* Adjusted [`windower.ffxi.get_bag_info`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiget_bag_info_bag) to work on the entire inventory when no argument is provided

2015-01-06
----------

LuaCore 1.8.1.7 - Arcon
* Fixed an issue where the entire bag was pushed instead of just its ID in the equipment table

2015-01-05
----------

Timers 3.6.2.2 - Arcon
* Added *Pummeler's Lorica* and *Agoge Calligae*/*+1* to *Berserk* duration calculations

LuaCore 1.8.1.6 - Arcon
* Efficiency improvements
  * [`windower.ffxi.get_mob_by_id`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start#windowerffxiget_mob_by_id_id) will now be constant time if the ID belongs to an NPC (pets included)

Timers 3.6.2.1 - Arcon
* Efficiency improvements

Timers 3.6.2.0 - Arcon
* Fixed targets disappearing when zoning
* Fixed crash when using the `timers` command with no arguments

2015-01-04
----------

Timers 3.6.1.6 - Arcon
* Adjusted display to fit larger fonts better and to not cut off text vertically
* Added comments to describe what certain settings do

Timers 3.6.1.5 - Arcon
* Fixed a bug where *Earthen Ward*'s and *Aerial Armor*'s duration would incorrectly benefit from summoning skill

Timers 3.6.1.4 - Arcon
* Added the *Evasionist's Cape*'s effect to *Embolden*
* Fixed a buff that would make enfeebling magic rules apply to blue magic

Timers 3.6.1.3 - Arcon
* Fixed *Diffusion* incorrectly boosting certain blua magic spells

Timers 3.6.1.2 - Arcon
* Fixed target names showing up as `Unknown`

Timers 3.6.1.1 - Arcon
* Added *Astral Conduit* merits into the calculations for *Blood Pact: Ward* durations

2015-01-03
----------

Timers 3.6.1.0 - Arcon
* Fixed durations for blood pact ward timers (did not consider summoning magic skill)

LuaCore 1.8.1.5 - Arcon
* Added `enabled_<bag>` keys for all bags to the table returned by [`windower.ffxi.get_items`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start#windowerffxiget_items_bag_index) when no bag is provided

LuaCore 1.8.1.4 - Arcon
* Added `enabled` key to the table returned by [`windower.ffxi.get_items`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start#windowerffxiget_items_bag_index) when a bag is provided

2015-01-02
----------

LuaCore 1.8.1.3 - Arcon
* Fixed a crash in `string.unpack` when used with bit-packed values
* Fixed `string.unpack` returning 0 when used with a 32-bit format specifier

Timers 3.6.0.0 - Arcon
* Added avatar blood pacts to buff duration timers
* Added support for certain *Dancer* and *Rune Fencer* job abilities that work differently from regular job abilities
* Made buff timers hold their countdown on zoning to reflect their real duration more accurately

2014
----

View older entries [here](https://github.com/Windower/Issues/blob/master/ChangeLog%202014.md).
