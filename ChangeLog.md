2016-02-10
----------

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
