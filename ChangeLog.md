2014-09-10
----------

LuaCore 1.7.12.7 - Arcon
* Fixed a bug in the IPC event handler

Timers 3.4.0.10 - Arcon
* Fixed after update

2014-09-09 September FFXI Update
----------

FFXIDB 0.9.1.8 - Arcon
* Fixed after update

LuaCore 1.7.12.6 - Arcon
* Fixed after update

BlinkMeNot 3.4.0.5 - Arcon
* Fixed after update

PetTP 2.2.0.6 - Arcon
* Fixed after update

2014-09-07
----------

Bidder 1.4.1.8 - Arcon
* Fixed a crash when typing malformed commands

2014-09-06
----------

Hook 4.2.8.2 - Arcon
* Fixed a bug that would cause the primitve and text object storage to become corrupted

LuaCore 1.7.12.5 - Arcon
* Fixed a bug that caused registered events to execute after the unload event

2014-09-05
----------

LuaCore 1.7.12.4 - Arcon
* Fixed a bug where addons that don't exist could erroneously be loaded

2014-08-31
----------

LuaCore 1.7.12.3 - Arcon
* Added the party changes from *1.7.12.0* back in

LuaCore 1.7.12.2 - Arcon
* Fixed a crash when calling `windower.ffxi.get_party()` before being logged in

LuaCore 1.7.12.1 - Arcon
* Reverted to *1.7.11.0*
  * Addons need to be changed first to be compatible to *1.7.12.0*

LuaCore 1.7.12.0 - Arcon
* Adjusted the party table
  * Added `party1_leader`, `party2_leader` and `party3_leader` as well as `alliance_leader`
    * Will all be `nil` if not applicable

2014-08-30
----------

Unlimited 1.0.1.0 - Arcon
* Defaulted to 60 FPS cap
* Added settings file with option to uncap the framerate completely

2014-08-28
----------

Unlimited 1.0.0.0 - Arcon - ***New plugin***
* Removes the game's native 30 FPS cap

Timers 3.4.0.9 - Motenten
* Removed debug changes introduced in *3.4.0.8*
* Internal changes to prevent possible crashes when creating/deleting timers

LuaCore 1.7.11.0 - Arcon
* Internal restructuring of the event handler
  * Avoids some crashes that occurred when an event was unregistered while the same event has been processing

2014-08-27
----------

Timers 3.4.0.8 - Motenten
* Added debug changes

2014-08-24
----------

Hook 4.2.8.1 - Arcon
* Fixed a crash on zoning introduced in *Hook 4.2.8.0*

2014-08-23
----------

LuaCore 1.7.10.0 - Arcon
* Fixed a bug which caused `windower.ffxi.get_mob_by_target('st')` to return `nil` despite a sub-target being active
* Fixed a bug which caused `windower.ffxi.get_mob_by_target('t')` to return the sub-target when no main target was active
* Added `'stpt'` and `'stal'` as options for `windower.ffxi.get_mob_by_target`
  * Will only work if `<stpt>` and `<stal>` were used respectively
  * `'st'` will return `nil` if `<stpt>` or `<stal>` are active

Hook 4.2.8.0 - Arcon
* Fixed a possible text-related crash
* Adjusted packet deduplication
  * Removed some more packets from the deduplicator
  * Made the queued packet list clear on zone
* Added *Banggugyangu*'s developer key

2014-08-21
----------

Timers 3.4.0.7 - Motenten
* Add Eminent Flute and Linos (plus augments) for song duration calculations.


2014-08-20
----------

LuaCore 1.7.9.5 - Arcon
* Fixed an issue which caused `windower.ffxi.get_mob_by_target('st')` to return nil despite a sub-target being active

2014-08-18
----------

Timers 3.4.0.6 - Motenten
* Set barspells to have a max duration of 30 minutes
* Allow gear enhancements to affect protect/shell spells
* Allow Composure to affect Klimaform


2014-08-15
----------

Timers 3.4.0.5 - Motenten
* Fix 0 recast crash issue


2014-08-12
----------

BlinkMeNot 3.1.0.4 - JoshK6656
* Built against party sig changing.

InfoBar 1.2.0.6 - JoshK6656
* Adjusted for party signature offset

SSOrganizer 1.5.1.6 - JoshK6656
* Removed random print (https://github.com/Windower/Issues/issues/586)

LuaCore 1.7.9.4 - JoshK6656
* Add new job points

Guildwork 1.4.2.7 - JoshK6656
* Built against party sig changing.

LuaCore 1.7.9.3 - JoshK6656
* Built against party sig changing.

TParty 1.2.2.8 - JoshK6656
* Built against party sig changing.

Timers 3.4.0.4 - Motenten
* Add Fealty adjustments
* Add Souleater adjustments


2014-08-07
----------

Timers 3.4.0.3 - Motenten
* Reset TargetMap tracking list when zoning.  Fixes issue of corrupted targets.
* Clear correct timers list when dead.
* Clean up and refactor packet inspection code.
* Use recast ID for selecting JA icons.


2014-08-06
----------

Timers 3.4.0.2 - Motenten
* Extra null check when checking target mob array for mob enemy type
* Override default buff ID of 0 for Boost


2014-08-05
----------

Timers 3.4.0.1 - Motenten
* Fix pointer reference which generated target name gibberish
* Fix check for whether an action target is a mob

Timers 3.4.0.0 - Motenten
* Add Nightingale/Troubadour buff duration gear
* Fix Circle buff duration gear for pld/drk
* Prevent Vivacious Pulse from generating spurious timers

2014-08-04
----------

Timers 3.3.0.8 - Motenten
* Fix bad pointer referencing that caused a crash

Timers 3.3.0.7 - Motenten
* When buffs wear off the player, remove them from the timer target list rather than deleting the timer itself

Timers 3.3.0.6 - Motenten
* Do not use existing bar durations when reusing an existing timer, as that leads to timer overlap
* When searching for existing buffs to replace, do not stop after the first one found
* Allow targets to be added to a timer (used when updating an existing timer)
* Do not create a timer that's going to be discarded when we just reuse an existing one

Timers 3.3.0.5 - Motenten
* Add new pref for sorting order (Creation, Duration, Alphabetical)
* Remove orderAlphabetically pref
* Fix pref names that were out of sync between load and save
* Fix pref names with buff/buffs prefix to all be buffs
* Prevent buff timers from being created for actions that target mobs
* Fix timer bar counter to increment, so that user limit prefs are adhered to

Timers 3.3.0.4 - Motenten
* Counting is hard

Timers 3.3.0.3 - Motenten
* Fix crash from accessing potentially null pointer

2014-08-02
----------

DelayMeNot 1.0.0.1 - Arcon
* Fixed a crash on unload

2014-08-01
----------

DelayMeNot 1.0.0.0 - Iryoku - ***New plugin***
* Removes the macro bar delay when using keyboard controls

Timers 3.3.0.2 - Arcon
* Fixed `orderAlphabetically` setting
  * It would display timers in reverse alphabetical order

Timers 3.3.0.1 - Arcon
* Fixed an issue where overwriting buffs would immediately be removed

Timers 3.3.0.0 - Arcon
* Recoded the target aspect of the plugin
  * Targets will now display more accurately
  * Buffs will only refresh if the same people are hit with it
    * Otherwise a new timer will pop up with the new people and the old timer will show less people on it
* Fixed an issue in text mode where the targets would not be displayed
* Further internal efficiency changes

Hook 4.2.7.3 - Arcon
* Fixed an issue where text objects would crash when being destroyed

2014-07-31
----------

Hook 4.2.7.2 - Arcon
* Fixed an issue where the incorrect plugin name would be displayed if a crash occurred on plugin load
* Some internal refactoring for primitive deletion 

Hook 4.2.7.1 - Arcon
* Fixed an issue where primitives would crash when being destroyed

2014-07-28
----------

Sandbox 1.0.1.5 - JoshK6656
* Fixed hook to work on Windows 8 along with Windows 7

LuaCore 1.7.9.2 - Arcon
* Fixed `tonumber` to work with negative numbers in bases other than `10`

LuaCore 1.7.9.1 - Arcon
* Added a `mog_house` `bool` to the `windower.ffxi.get_info` table
  * Requires *Hook 4.2.7.0*

LuaCore 1.7.9.0 - SnickySnacks
* Added [`windower.ffxi.get_bag_info`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiget_bag_info_bag)
  * Requires *Hook 4.2.7.0*

Hook 4.2.7.0 - SnickySnacks
* Added mog house tracking
* Added inventory enabling tracking

Hook 4.2.6.4 - Arcon
* Minor internal cleanup to help with debugging

2014-07-27
----------

Attainment 2.2.6.8 - Snicky
* Fix Dynamis and Abyssea offsets. 
* Fix zoning not clearing Abyssea/Dynamis info. 
* Added tracking of Dynamis KIs upon login.

2014-07-25
----------

Hook 4.2.6.3 - Arcon
* Removed some packets from the deduplication mechanism to potentially fix a bug

2014-07-24
----------

Timers 3.2.0.1 - Arcon
* Fixed an issue where *Timers* would crash with `graphicalMode` set to `false`
* Fixed the text offset so the text doesn't overlap with `graphicalMode` set to `false`

Timers 3.2.0.0 - Arcon
* Made the plugin parse the Lua resources
  * This means we only have to maintain the buff durations in one resource branch
  * *Timers* will now work immediately after the first resource fix after a FFXI update, since we always update Lua resources first

LuaCore 1.7.8.3 - Arcon
* Fixed `windower.regex.match` only returning the first match instead of all
* Minor efficiency improvements of `windower.regex` functions

Timers 3.1.2.2 - Motenten
* Fixed custom timers overwriting different custom timers

Timers 3.1.2.1 - Arcon
* Fixed certain buffs not being refreshed correctly

Timers 3.1.2.0 - Arcon
* Enabled custom timer commands

Timers 3.1.1.0 - Arcon
* Fixed buffs not overwriting the same buff
* Made exceptions for BRD songs, they will now update if cast again with a higher duration

Timers 3.1.0.0 - Arcon, Motenten
* Fixed recast icons being displayed
  * Added different icons for SP abilities depending on the job
* Fixed Stratagem count
* Fixed flashing issues
  * The entire bar instead of just the border would flash
  * Any suffix the name had would be lost (such as `[Self]` on self-targeted buffs)
* Losing a buff will now cancel the lowest timer for that particular buff
* Fixed a deadlocking issue and improved performance a bit
* Fixed timers not always moving up when space was available
  * They would move up when they were canceled but not when they expired naturally
* Fixed some calculations:
  * Made *Protect*/*Shell* not be affected by *Composure*
  * Fixed the *Grapevine Cape*'s effect to only work on self-targeted buffs
  * Fixed multipliers for song durations

2014-07-23
----------

Timers 3.0.0.0 - Arcon
* Massive recode
  * Changed how timers work internally to avoid several bugs in the previous version
  * Fixed some display issues
    * Timers not moving up when space previous timers disappear
    * Timers displaying incorrect or inverted colors
    * Timers not flashing correctly when expiring
  * Added various new settings
* Note this is still only a test version and some things are known not to work (like *Stratagem* count) which is why this is a dev-release only and will not go live until it has been further tested and the missing features implemented

Hook 4.2.6.2 - Arcon
* Fixed a possible crash source when deleting primitives

Hook 4.2.6.1 - Arcon
* Fixed the order in which primitives are rendered
  * It is now, as it used to be before *4.2.6.x*, the order in which they are created in

2014-07-22
----------

Hook 4.2.6.0 - Arcon
* Fixed minor primitive bug
* Refactored the primitive handler, made efficiency improvements and added safeguards
* Implemented text and primitive deletion by object in addition to deletion by string

2014-07-20
----------

Timers 2.0.4.3 - Arcon
* Fixed Timers disappearing issue from *2.0.3.0*, re-enabled recasts clearing when they disappear

Timers 2.0.4.2 - Arcon
* Fixed a freezing issue and buffs wear off, as well a possible crash source

Timers 2.0.4.1 - Arcon
* Reverted the *2.0.3.0* change because a new bug appeared where incorrect timers would show up

Timers 2.0.4.0 - Arcon
* Made buff timers wear off when a buff disappears

Timers 2.0.3.0 - Arcon
* Made recast timers wear off if they suddenly disappear (like when changing jobs)

Timers 2.0.2.3 - Motenten
* Added reforged relic items to buff duration calculations
* Various fixes

Timers 2.0.2.2 - Arcon
* Added *Diffusion* effect to blue magic calculations

LuaCore 1.7.8.2 - SnickySnacks
* Fixed crashes when the stack grow too high

2014-07-18
----------

Timers 2.0.2.1 - Arcon
* Fixed text position in slim mode

Timers 2.0.2.0 - Arcon
* Adjusted to work from new resources
  * Moved buff duration in resources from `status.xml` to `abils.xml` and `spells.xml`

Timers 2.0.1.4 - Arcon
* Added missing adjustments to *Regen*

Timers 2.0.1.3 - Arcon
* Added jigs

Timers 2.0.1.2 - Arcon
* Added *RUN* job abilities

Timers 2.0.1.1 - Arcon
* Added *Gekka: Ichi*,  *Yain: Ichi* and *Crusade*

Timers 2.0.1.0 - Arcon
* Fixed bar direction for the `lowToHigh` setting `true`
* Minor efficiency improvements, code cleanup

Hook 4.2.5.8 - Arcon
* Adjusted developer keys

2014-07-16
----------

Timers 2.0.0.1 - Arcon
* Fixed a buff where certain JA buffs would not show up correctly

Timers 2.0.0.0 - Arcon
* Full recode
  * Fixed a few remaining graphical issues, like colors being inverted and mid and final color being reversed
  * Adjusted buff duration format to be more flexible and allow for further adjustments
    * The old format was not able to implement all buff effects correctly
    * Buffs with multiple multipliers and additions could not be modeled

2014-07-15
----------

LuaCore 1.7.8.1 - Arcon
* Minor efficiency improvement

LuaCore 1.7.8.0 - Arcon
* Added [`windower.packets.parse_action`](http://dev.windower.net/doku.php?id=lua:api:functions:packets:start&#windowerpacketsparse_action_payload) function
* Deprecated the `action` event

2014-07-13
----------

Guildwork 1.4.2.6 - SnickySnacks
* Fixed a crash source on logout

Hook 4.2.5.7 - Arcon
* Adjusted developer keys

2014-07-12
----------

AutoExec 2.8.1.5 - Arcon
* Fixed for new resources

StatusTimer 1.2.2.8 - Arcon
* Fixed for new resources

Bidder 1.4.1.7 - Arcon
* Fixed for new resources

SSOrganizer 1.5.1.5 - Arcon
* Fixed for new resources

Spellcast 2.6.2.19 - Arcon
* Fixed for new resources

GearCollector 1.0.4.6 - Arcon
* Fixed for new resources

Itemizer 1.2.3.5 - Arcon
* Fixed for new resources

Find 1.0.5.5 - Arcon
* Fixed for new resources

2014-07-10
----------

Guildwork 1.4.2.5 - Arcon
* Rebuilt against new API

FFXIDB 0.9.1.7 - Arcon
* Rebuilt against new API

TParty 1.2.2.7 - Arcon
* Rebuilt against new API

Timers 1.2.2.3 - Arcon
* Rebuilt against new API

Launcher 4.2.5304.40974 - Iryoku
* Fixed an issue where an outdated `addons.json` file would be retrieved, preventing addon updates

LuaCore 1.7.7.9 - Arcon
* Fixed an issue with the `pack` library
  * The `A` code didn't behave correctly when trying to pack a string. The numeric modifier acted as an array indicator instead of a string length indicator
* Fixed a possible crash when having too many buffs

Hook 4.2.5.6 - Arcon
* Fixed an issue where weather would occasionally be overwritten by an incorrect value

2014-07-09
----------

FFXIDB 0.9.1.6 - Arcon
* Fixed missing map display in *Ordelle's Caves*
* Fixed displaying the wrong map (of *Ordelle's Caves*) in *Outer Horutoto Ruins*

2014-07-08 July FFXI Update
----------

LuaCore 1.7.7.8 - Arcon
* Fixed party table from `windower.ffxi.get_party`

TParty 1.2.2.6 - Arcon
* Fixed after update

2014-07-06
----------

LuaCore 1.7.7.7 - Arcon
* Fixed a potential crash in `cancel_buff`
* Fixed incorrect buff-related checks when 32 buffs were active

2014-07-05
----------

Hook 4.2.5.5 - Arcon
* Added a `console_fadespeed` command
  * Sets the time it takes for the console to fade out (unlike `console_fadedelay`, which sets the time at which it *starts* fading out)
  * Takes the number of frames it should last, default being 25

LuaCore 1.7.7.6 - Arcon
* Added some debugging options to the dev version

2014-07-04
----------

TParty 1.2.2.5 - Cair
* Removed text objects that display alliance MP amounts.

2014-07-03
----------

LuaCore 1.7.7.5 - Arcon
* Improved error checking in the `pack` module to prevent accessing junk memory, specifically when working with custom bit boundaries

LuaCore 1.7.7.4 - Arcon
* Fixed an issue in the `pack` module
  * `q` will now only cover one bit
    * If a numeric value is specified, it will return that number of values of sequential boolean bits
    * Defaults to 1
  * `string.unpack` now takes an optional fourth value which indicates which bit to start from
    * Only works for `b` and `q`, otherwise it will round up to the next multiple of 8

2014-07-01
----------

Guildwork 1.4.2.4 - JoshK6656
* Rebuilt against new API to include job points

2014-06-27
----------

Timers 1.2.2.2 - Arcon
* Adjusted to new Hook API

LuaCore 1.7.7.3 - Arcon
* Adjusted to new Hook API, fixed equipment bags

Hook 4.2.5.4 - Arcon
* Fixed an issue in the plugin interface (equipment bags were mismatched)

2014-06-26
----------

Hook 4.2.5.3 - Iryoku
* Fixed unhandled commands not being passed to the 3.x MMF console handler

LuaCore 1.7.7.2 - Motenten, Arcon
* Fixed various spelling issues in the job points table
  * `jobp_oints` renamed to `job_points`
  * `avatarspirit_accuracy_bonu` renamed to `avatar_spirit_accuracy_bonus`
  * `avatarspirit_mag_acc_bonus` renamed to `avatar_spirit_magic_accuracy_bonus`

Timers 1.2.2.1 - Arcon
* Fixed an issue where the recast times would be cut off in text mode

Hook 4.2.5.2 - Arcon
* Made job points populate correctly before opening the menu the first time

LuaCore 1.7.7.1 - Arcon
* Renamed `jobpoints` to `job_points` in the player table

Hook 4.2.5.1 - Arcon
* Fixed job point parsing

2014-06-25
----------

FFXIDB 0.9.1.5 - Arcon
* Fixed radar not displaying in *La Vaule [S]*

Timers 1.2.2.0 - Arcon
* Added *Clarion Call* job points for BRD songs

2014-06-24
----------

LuaCore 1.7.7.0 - JoshK6656, Arcon
* Added job points to the player table

Hook 4.2.5.0 - Arcon
* Added job point info to the *ExtData* interface

2014-06-23
----------

Timers 1.2.1.1 - Arcon
* Adjusted it to only remove self-targeted buffs upon death

Timers 1.2.1.0 - Arcon
* Made all buffs clear upon death

Timers 1.2.0.0 - Arcon
* Implemented various new settings
  * `textColoring`
    * Will color text as it colors the bars in graphical mode
    * Works in both graphical and text mode
  * `flashDuration`
    * Sets the duration (in seconds) of how long the bar should flash after the timer wears off
  * `medPercent`/`lowPercent`
    * Sets the percentage at which the plugin should switch into medium/low HP (used for coloring)
* Will now cut off the text if it's too long as to not overlap with the displayed duration

Hook 4.2.4.0 - Arcon
* Implemented explit text size setting

2014-06-19
----------

LuaCore 1.4.6.2 - JoshK6656
* Fixed AGI, INT and MND merits

LuaCore 1.4.6.1 - Arcon
* Added GEO and RUN merits

LuaCore 1.4.6.0 - JoshK6656
* Added `maximum_merit_points` to the merit struct

2014-06-17 June FFXI Update
----------

FFXIDB 0.9.1.4 - Arcon
* Fixed map display in Cirdas Caverns

TParty 1.2.2.4 - Arcon
* Adjusted TP coloring to correct for the new values

2014-06-16
----------

LuaCore 1.4.5.0 - JoshK6656
* Adjusted spawn type to incorporate Trust NPCs
  * This affects the `in_party` and `in_alliance` fields for Trust NPCs, which displayed incorrect information before

2014-06-10
----------

FFXIDB 0.9.1.3 - Arcon
* Fixed a crash when trying to set custom ranges

2014-06-09
----------

FFXIDB 0.9.1.2 - Arcon
* Fixed an issue where the map would stay hidden after zoning back out of a Mog House

2014-06-07
----------

LuaCore 1.7.4.0 - Arcon
* Fixed major memory leak on reloading LuaCore
* Fixed a bug where `unload` events would not always be called when unloading addons or reloading LuaCore

LuaCore 1.7.3.4 - Arcon
* Fixed `gain buff` and `lose buff` events in case of multiple buffs with the same ID

2014-06-05
----------

LuaCore 1.7.3.3 - Arcon
* Temporarily reverted `gain buff` and `lose buff` changes as they seemed to cause unexpected issues

LuaCore 1.7.3.2 - Arcon
* Added `heading` to the mob struct, identical to `facing`
* Deprecated the `facing` field in the mob struct in favor of `heading`
  * Support for `facing` will be dropped soon, so no new addons should be using it

LuaCore 1.7.3.1 - Arcon
* Fixed `gain buff` and `lose buff` events in case of multiple buffs with the same ID

2014-06-03
----------

Hook 4.2.3.1 - Arcon
* Fixed a bug where only the last key item packet would be considered

LuaCore 1.7.3.0 - Arcon
* Added [`windower.ffxi.get_key_items`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiget_key_items) which returns a list of available key items

Hook 4.2.3.0 - Arcon
* Added key item recording

2014-05-30
----------

Launcher 4.2.5263.39744 - Arcon
* Will now create a settings folder for plugins, if plugins are downloaded

2014-05-29
----------

LuaCore 1.7.2.0 - Arcon
* Adjusted [`coroutine.schedule`](http://dev.windower.net/doku.php?id=lua:api:functions:start#coroutineschedule_fn_time)
  * Will now also accept an existing coroutine instead of a function
  * Will return the scheduled coroutine
* Added [`coroutine.close`](http://dev.windower.net/doku.php?id=lua:api:functions:start&#coroutineclose_co)
  * Will close coroutines by LuaCore (as opposed to coroutines created from within a Lua file)
  * Closed coroutines will never execute again and cannot be resumed

2014-05-27
----------

FFXIDB 0.9.1.1 - Arcon
* Removed debug message

LuaCore 1.7.1.1 - Arcon
* Fixed `windower.ffxi.get_map_data` and `windower.ffxi.get_position`
  * It was working fine most of the time but had issues in certain parts of certain zones

FFXIDB 0.9.1.0 - Arcon
* Fixed map display in every zone

2014-05-27
----------

LuaCore 1.7.1.0 - Arcon
* Changed [`coroutine.sleep`](http://dev.windower.net/doku.php?id=lua:api:functions:start#coroutinesleep_time) and [`coroutine.schedule`](http://dev.windower.net/doku.php?id=lua:api:functions:start#coroutineschedule_fn_time) to use seconds instead of milliseconds
* Fixed a bug that caused stack corruption when sleeping/yielding and possibly crashed POL

LuaCore 1.7.0.0 - Arcon
* Removed `windower.sleep`
* Added [`coroutine.sleep`](http://dev.windower.net/doku.php?id=lua:api:functions:start#coroutinesleep_time)
  * Sleeps the current evaluation for the given number of milliseconds
  * It will never block the game and never block other calls/functions of the same addon
  * If called from inside an event, will function as a return
    * Any return values after the sleep will be ignored
    * `coroutine.yield` should be used to return values before a call to `coroutine.sleep`
* Added [`coroutine.schedule`](http://dev.windower.net/doku.php?id=lua:api:functions:start#coroutineschedule_fn_time)
  * Schedules a function to run in the given number of milliseconds
* `coroutine.yield` when now called from inside an event will function similar to a return
  * Allows the event call to continue to the next addon
  * The provided arguments will be treated as return values
  * The function will then be resumed on its own time afterwards without disrupting the event chain

2014-05-25
----------

LuaCore 1.6.5.4 - Arcon
* Fixed deadlock on startup

LuaCore 1.6.5.3 - Arcon
* Fixed vertical distance in `windower.text.get_extents`

FFOChat 1.1.0.4 - Arcon
* Added Unicode support (in the scope of FFXI's native Shift_JIS)

2014-05-23
----------

LuaCore 1.6.5.2 - Arcon
* Added two functions to `windower`:
  * [`to_shift_jis`](http://dev.windower.net/doku.php?id=lua:api:functions:start&#windowersleep_time) Converts a UTF-8 string to Shift_JIS
  * [`from_shift_jis`](http://dev.windower.net/doku.php?id=lua:api:functions:start&#windowerfrom_shift_jis_str) Converts a Shift_JIS string to UTF-8

2014-05-21
----------

Timers 1.1.5.3 - Arcon
* Fixed buff names with shared recasts being mixed up

2014-05-20
----------

Timers 1.1.5.2 - Arcon
* Fixed JA buff names being displayed incorrectly

LuaCore 1.6.5.1 - Arcon
* Fixed text box dragging mechanics

Launcher 4.2.5253.20271 - Arcon
* Fixed bug where resources would be checked even when they weren't changed

Timers 1.1.5.1 - Arcon
* Fixed Stratagem count (hopefully for real this time)

2014-05-19
----------

Launcher 4.2.5252.20750 - Arcon
* Fixed bug where resources would be deleted upon download

Launcher 4.2.5252.16592 - Arcon
* Fixed bug where resources would be downloaded even when they weren't updated

2014-05-17
----------

LuaCore 1.6.5.0 - Arcon
* Changed [`windower.ffxi.get_abilities`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiget_abilities)
  * Now returns a table with 4 sub-tables:
    * `job_abilities`
    * `job_traits`
    * `weapon_skills`
    * `pet_commands`
  * Each of the sub-tables is a list of IDs of the respective category that your current character has access to

Launcher 4.2.5250.31346 - Arcon
* Adjusted the launcher to clean up unneeded resource files

LuaCore 1.6.4.0 - Arcon
* Improved [`windower.ffxi.get_items`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiget_items_bag_index) interface

2014-05-15
----------

Timers 1.1.5.0 - Arcon
* Adjusted to read equipment data from *Wardrobe*

GearCollector 1.0.4.5 - Arcon
* Adjusted to new inventory structure

LuaCore 1.6.3.3 - Arcon
* Fixed an error where [`windower.ffxi.set_equip`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiset_equip_inv_id_slot_bag) would not accept a third argument

2014-05-14 May FFXI update
----------

LuaCore 1.6.3.2 - Arcon
* Adjusted [`windower.ffxi.get_abilities`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiget_abilities) due to a changed packet

Find 1.0.5.4 - JoshK6656
* Added *Wardrobe* support

Itemizer 1.2.3.4 - JoshK6656
* Disabled attempts to set/get non-equipment items from *Wardrobe*

LuaCore 1.6.3.1 - Arcon
* Fixed an error where `slot_bag` for the various slots wasn't populated correctly

LuaCore 1.6.3.0 - Arcon
* Fixed [*Equipment*](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiget_items), finalized wardrobe changes
* Equipment now has two values for each slot (`main`, `sub`, `range`, etc.):
  * `slot`: The inventory index of the item in that slot
  * `slot_bag`: The inventory bag the item in that slot is in
    * Only `0` and `8` valid for *Inventory* and *Wardrobe* respectively

Itemizer 1.2.3.3 - JoshK6656
* Added *Wardrobe* support

Hook 4.2.2.0 - Arcon
* Added wardrobe-related equipment information

LuaCore 1.6.2.2 - Arcon
* Enabled [`windower.ffxi.set_equip`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiset_equip_inv_id_slot_bag) with optional third argument for inventory bag
* Added `wardrobe` for all categories in the `items` table:
  * `wardrobe`
  * `max_wardrobe`
  * `count_wardrobe`

LuaCore 1.6.2.1 - Arcon
* Disabled [`windower.ffxi.set_equip`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiset_equip_inv_id_slot_bag) to examine effects of update


Hook 4.2.1.14 - Arcon
* Preliminary adjustment for inventory expansion

2014-05-13
----------

LuaCore 1.6.2.0 - Arcon
* Fixed typo (`entity_type` in the mob table was mistakenly named `Entity_type`)
* Added `models` to the mob table
  * It's an array starting at 1 and going until the models for a mob run out
  * PCs have the following models:
    * 1: Face
    * 2: Head
    * 3: Body
    * 4: Hands
    * 5: Legs
    * 6: Feet
    * 7: Main
    * 8: Sub
    * 9: Ranged
  * Most mobs only have one value, some NPCs have multiple values

2014-05-12
----------

LuaCore 1.6.1.13 - Arcon
* Fixed error messages cutting off too much of the path
  * Only happened when the `CondenseError` LuaCore option was set to `true`

2014-05-11
----------

LuaCore 1.6.1.12 - Arcon
* Fixed an error where the level-up event would trigger on login or job change
  * Another such error persists and will be adjusted shortly

2014-05-10
----------

LuaCore 1.6.1.11 - Arcon
* Removed debug message

LuaCore 1.6.1.10 - Arcon
* Adjusted all screen coordinates for UI scaling
* Fixed the job change event from triggering on login
* Changed the `status` value of the player table to contain the status ID instead of the name
* Changed the `action message` event signature
  * Parameters 2 and 3 are now merged into one

2014-05-05
----------

LuaCore 1.6.1.9 - Arcon
* Fixed crafting skills being returned incorrectly
* Changed `guarding` to `guard`

2014-05-04
----------

Hook 4.2.1.13 - Arcon
* Video encoding will now upscale resolution to the next multiple of `4` instead of failing

2014-05-02
----------

JaZero 1.2.2.7 - Arcon
* Fixed crash during home point set dialogue after a job change

LuaCore 1.6.1.8 - Arcon
* Adjusted mob table
  * Changed `model_size` to `model_scale`
  * Added actual `model_size`

LuaCore 1.6.1.7 - Arcon
* Added [`windower.ffxi.drop_item`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxidrop_item_index_count) function

LuaCore 1.6.1.6 - Arcon
* Added the following skills to the `skills` table
  * `geomancy`
  * `handbell`

LuaCore 1.6.1.5 - Arcon
* Renamed the following skill names in the `skills` table to match the in-game names better
  * `divine` to `divine_magic`
  * `enhancing` to `enhancing_magic`
  * `elemental` to `elemental_magic`
  * `enfeebling` to `enfeebling_magic`
  * `dark` to `dark_magic`
  * `summoning` to `summoning_magic`
  * `string` to `stringed_instrument`
  * `wind` to `wind_instrument`

LuaCore 1.6.1.4 - Arcon
* Renamed `ninjitsu` to `ninjutsu` in the `skills` table, as it is in-game

FFOChat 1.1.0.3 - Arcon
* Fixed name display when receiving PMs

FFOChat 1.1.0.2 - Arcon
* Fixed crash on receiving PMs
* Fixed crash when failing to connect to a server

2014-05-01
----------

Launcher 4.2.5234.31468 - Arcon
* Adjusted resources
  * Moved hardcoded resources into the [ResourceExtractor](https://github.com/Windower/ResourceExtractor) repository
  * Fixed resources bug
* Added separate resource directory for the Windower development build

2014-04-28
----------
LuaCore 1.6.1.3 - Cair
* Added `target_index` to the mob array structure. This is always 0 for NPCs.


2014-04-27
----------

Launcher 4.2.5230.31708 - Arcon
* Adjusted to download resources before plugins
  * Otherwise running instances may reload plugins before new resources have been downloaded

Launcher 4.2.5230.11240 - Arcon
* Added all missing Lua resources to the Launcher
* Changed the format of the server manifest to disambiguate resources of different types

2014-04-26
----------

UpdateResources *discontinued* - Arcon
* Resources will now be downloaded through the Windower Launcher
* The plugin is still functional and will not be removed from the plugins folder
* It will, however, no longer be downloaded through the Launcher

Launcher 4.2.5229.33144 - Arcon
* Included plugin resources into the resource downloader

Launcher 4.2.5229.33144 - Arcon, Iryoku
* Added resource downloader

LuaCore 1.6.1.2 - Arcon
* Added [`windower.windower_path`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start) variable

LuaCore 1.6.1.1 - Arcon
* Adjusted [`windower.ffxi.get_mob_name`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiget_mob_name_index) function to work with an ID instead of index
* Reduced file size and load speed by removing unsued dependencies and functions

2014-04-25
----------

LuaCore 1.6.1.0 - Arcon
* Added [`windower.ffxi.get_mob_name`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start&#windowerffxiget_mob_name_index) function

Spellcast 2.6.2.18 - Arcon
* Fixed crash on using the `sc group` command

Hook 4.2.1.12 - Arcon
* Added console logging
  * Off by default, toggle with `console_log [0|1]`

Attainment 2.2.6.7 - Arcon
* Fixed crash on load bug

LuaCore 1.6.0.0 - Suji, Iryoku
* Added the `LuaSocket` library

Attainment 2.2.6.6 - Arcon
* Fixed various bugs to tracking merits

LuaCore 1.5.4.3 - Arcon
* Added `species` and `instincts` to `windower.ffxi.get_mjob_data` and `windower.ffxi.get_sjob_data` when on Monipulator

Hook 4.2.1.11 - Arcon
* Fixed video recording

Hook 4.2.1.10 - Arcon
* Fixed mouse coordinates when playing windowed

2014-04-24
----------

LuaCore 1.5.4.2 - Arcon
* Adjusted shortened error display
* Fixed shortened errors on loading plugins

2014-04-20
----------

Spellcast 2.6.2.17 - Arcon
* Fixed another issue with `sc var set` where it would omit spaces under certain conditions

2014-04-19
----------

Find 1.0.5.3 - Arcon
* Fixed gil slot being ignored for item tracking

Spellcast 2.6.2.16 - Arcon
* Fixed issue with `sc var set` where it wouldn't parse the entire line

LuaCore 1.5.4.1 - Arcon
* Fixed addon load text display

LuaCore 1.5.4.0 - Arcon
* Fixed incorrect triggering of the `status change` event immediately after logging in
* Added fishing (`50`) and event (`4`) to the list of events which status change will trigger on

LuaCore 1.5.3.3 - Arcon
* Fixed unload crash
* Prettied up loading text for addons
  * Author and version will now only be displayed if set

Find 1.0.5.2 - Arcon
* Fixed issue where tracking certain items would display the number of used slots in the inventory instead of the actual item count

2014-04-17
----------

Timers 1.1.4.8 - Arcon
* Added `Shabti Cuirass` and `Shabti Cuirass +1` to the calculations

2014-04-16
----------

Timers 1.1.4.7 - Arcon
* Fixed stratagem display (again)

2014-04-15
----------

WeatherMon 1.0.1.8 - JoshK6656
* Fixed the weather tracking

LuaCore 1.5.3.3 - Arcon
* Fixed a crash source when using `windower.ffxi.turn`

LuaCore 1.5.3.2 - Arcon
* Fixed the `unhandled command` event providing the first argument twice

WeatherMon 1.0.1.7 - Arcon
* Fixed lightning not being recognized correctly (both day and weather)

Hook 4.2.1.9 - Arcon
* Added weather change packet to data extraction

Spellcast 2.6.2.15 - Arcon
* Fixed debugging

LuaCore 1.5.3.1 - Arcon
* Fixed debugging

2014-04-14
----------

LuaCore 1.5.3.0 - Arcon
* Added an escape character (`\`) to command handling
  * This allows to input double quotes into commands by prepending a `\`
  * Example: `//send mulename /item \"Stalwart's Tonic\" <me>`
  * Currently `"` and ` ` are the only escapeable characters, more may be added

2014-04-13
----------

Itemizer 1.2.3.2 - Arcon
* Fixed issue where only lower case commands were recognized by the plugin

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

