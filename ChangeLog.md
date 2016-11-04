2016-11-04
----------

Timers 3.7.4.13 - Arcon
* Added some bard gear to factor into buff duration calculations

2016-09-19
----------

LuaCore 2.0.4.7 - Arcon
* Fixed possible crashing issue when zoning

2016-07-16
----------

LuaCore 2.0.4.6 - Arcon
* Fixed an error in `windower.ffxi.get_player().in_combat`

2016-07-07 July FFXI Update
----------

Guildwork 1.4.3.2 - Arcon
* Adjusted to new API

Timers 3.7.4.12 - Arcon
* Adjusted to new API

LuaCore 2.0.4.5 - Arcon
* Adjusted to new API
* Added new inventories (`wardrobe3` and `wardrobe4`) to [`windower.ffxi.get_items`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start#windowerffxiget_items_bag_index) and [`windower.ffxi.get_bag_info`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start#windowerffxiget_bag_info_bag)

Hook 4.2.13.11 - Arcon
* Added two new inventories from the July update

2016-06-23
----------

LuaCore 2.0.4.4 - Arcon
* Fixed an issue with pasting text and setting chat input
* Added the function [`is_open`](http://dev.windower.net/doku.php?id=lua:api:functions:chat:start#windowerchatis_open) to the `windower.chat` table.

Hook 4.2.13.10 - Arcon
* Fixed an issue where pasting would not immediately update the chat box with the right value

2016-06-22
----------

LuaCore 2.0.4.3 - Arcon
* Fixed an issue where the `target_locked` property would always return `true`
* Fixed an issue where certain key items would not be listed

2016-05-16
----------

Timers 3.7.4.11 - Arcon
* Fixed an issue where SP abilities would display in English on the Japanese client
* Fixed the spelling of *Asylum*

Guildwork 1.4.3.1 - Arcon
* Fixed an issue where the game would freeze under heavy battle

2016-04-19
----------

Guildwork 1.4.3.0 - Arcon
* Added new type of kills to the FFXIDB collection mechanism

2016-04-14
----------

Hook 4.2.13.9 - Arcon
* Fixed a bug where certain items would remain in the *Using* state

2016-04-05 April FFXI Update
----------

Guildwork 1.4.2.13 - Arcon
* Added Wardrobe 2

Timers 3.7.4.10 - Arcon
* Added Wardrobe 2

LuaCore 2.0.4.2 - Arcon
* Added Wardrobe 2

Hook 4.2.13.8 - Arcon
* Added Wardrobe 2

2016-02-10 February FFXI Update
----------

FFXIDB 0.9.2.12 - Arcon
* Fixed for update

LuaCore 2.0.4.1 - Arcon
* Fixed for update

Hook 4.2.13.7 - Arcon
* Refactored packet handling to improve performance and maintainability
* Fixed key bindings for shift (using the tilde `~` key)

2016-02-08
----------

Timers 3.7.4.9 - Arcon
- Fixed an issue where "Enh. Mag. eff. dur." augment was not calculated correctly

2016-01-24
----------

FFXIDB 0.9.2.11 - Arcon
* Efficiency improvements
* Fixed an issue where the map positions would occasionally stutter by small amounts

LuaCore 2.0.4.0 - Arcon
* Added [`postrender`](http://dev.windower.net/doku.php?id=lua:api:events:start&#event_list) event
* Fixed [`windower.ffxi.get_info`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start#windowerffxiget_info) to return the correct server value (now matches the server ID from the [server resources](https://github.com/Windower/Resources/blob/master/xml/servers.xml))
* Fixed a crash when passing invalid values to [`windower.ffxi.get_mob_by_id`](http://dev.windower.net/doku.php?id=lua:api:functions:ffxi:start#windowerffxiget_mob_by_id_id)

2016-01-08
----------
LuaCore 2.0.3.1 - Cair
* Fixed errors relating to `add item` and `remove item` events

Config 2.0.1.2 - Cair
* Fixed a crash in command handling

2015
----

View older entries [here](https://github.com/Windower/Issues/blob/master/ChangeLog%202015.md).
