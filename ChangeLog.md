2017-06-30
----------

Chatmon 1.10.0.6 - Cair
* Fixed an issue where having chatmon loaded prevented `setkey` from working in certain situations

2017-06-13
----------

Hook 4.3.2.1 - Cair
* Fixed an issue that prevented other processes from accessing the clipboard
* Addressed a possible cause of multiple process zoning deadlocks
* Got a cool version number

2017-05-29
----------

LuaCore 2.1.0.2 - Arcon
* Fixed an issue when calling `print` with multiple arguments

2017-05-27
----------

Guildwork 1.4.3.5 - Byrth and Cair
* Fixed a crash caused by having an invalid Party pointer at logout.

Guildwork 1.4.3.4 - Byrth
* Removed the guildwork.com check for the "guildwork.dll" component of the guildwork plugin.

2017-05-24
----------

LuaCore 2.1.0.1 - Arcon
* Adjusted `windower.ffxi.get_player().jobs` to show `0` for jobs that are not unlocked

LuaCore 2.1.0.0 - Arcon
* Updated the code base to new standards, plugin-wide refactoring
* Adjusted `windower.ffxi.get_player().jobs` to only show levels for unlocked jobs, instead of displaying `1`

Hook 4.3.2.0 - Arcon
* Fixed an issue with pasting into the console
* Added tracking of job availability

2017-05-15
----------

Hook 4.3.1.1 - Cair
* Address several crashes on exiting to POL

2017-05-14
----------

Hook 4.3.1.0 - Cair
* Fix window retaining frame when toggled in windowed mode
* Fix the use of setkey while out of focus (again)
* Fix the use of Windows Key binds with multiple instances running

2017-05-08
----------

Hook 4.3.0.17 - Cair
* Fix stuck keyboard input after window changes

Hook 4.3.0.16 - Cair
* Prevent keyboard input delay after changing windows
* Fix Always Enable Sound/Always Enable Gamepad launcher settings

Launcher 4.3.6332.35270 - Cair
* Change settings handling for compatability with hook

2017-05-07
----------

Hook 4.3.0.15 - Cair
* Prevent controller device input delay after changing windows

Hook 4.3.0.14 - Cair
* Disable keyboard input while window is in background

2017-05-06
----------

Hook 4.3.0.13 - Cair
* Version bump - versioning mistake with pushed version

Hook 4.3.0.12 - Cair
* Reimplement mouse input delay fix

2017-05-05
----------

Hook 4.3.0.11 - Cair
* Fixed the use of setkey while out of focus

Hook 4.3.0.10 - Iryoku
* Enabled binds that use the windows key

2017-05-04 
----------

Hook 4.3.0.9 - Iryoku
* Fixed controller blocking method

Hook 4.3.0.8 - Cair
* Fixed loss of binds on window change

2017-05-03
----------

Launcher 4.3.6332.35270 - Iryoku
* Fixed hook injection method

Hook 4.3.0.7 - Iryoku
* Fixed stuck key inputs on window change
* Fixed controller focus behavior

2017-05-02 
----------
Timers 3.7.4.23 - Cair
* Fixed a crash caused by casting an AoE Buff on a character before it has loaded into memory.

2017-04-28 
----------

Hook 4.3.0.6 - Iryoku
* Fixed mouse delay with POL open

Hook 4.3.0.5 - Iryoku
* Fixed keyboard delay with POL open

2017-04-17
----------

Hook 4.3.0.4 - Arcon
* Fixed crash when playing sounds

2017-04-15
----------

Hook 4.3.0.3 - Arcon
* Fixed crash on creating primitive objects from addons

2017-04-14
----------

Hook 4.3.0.2 - Iryoku
* Fixed window/process name showing the currently logged in character

2017-04-13
----------

Hook 4.3.0.1 - Arcon
* Fixed crash when using certain Windower commands
* Fixed crash when using certain FFXI commands that were modified by addons

Launcher 4.3.6312.40615 - Iryoku
* Updated for new Hook

Hook 4.3.0.0 - Iryoku
* Refactored to use new hooking library to work with Windows 10 Creator's Update
* Further internal refactoring and fixed various related crashes

2017-04-06
----------

LuaCore 2.0.5.0 - Arcon
* Updated LuaSocket to version 3 RC1

2017-04-05
----------

LuaCore 2.0.4.10 - Arcon
* Fixed possible crash when using `windower.ffxi.get_mob_by_target` with `<scan>`

Timers 3.7.4.22 - Byrth
* Added buff calculations for *Inyanga Shalwar +2*

2017-04-03
----------

Sandbox 1.0.1.8~9 - Byrth
* Ensured that characters on the same computer will zone at least 100ms apart

2017-03-01
----------

Timers 3.7.4.21 - Byrth
* Added buff calculations for *Brioso Whistle* and *Moonbow Whistle* (*+1*)

2017-02-16
----------

Timers 3.7.4.20 - Byrth
* Added buff calculations for *Oranyan*, *Ammurapi Shield*, *Erilaz Galea* (*+1*)
* Fixed issues with previous duration calculations for RDM

2016
----

View older entries [here](https://github.com/Windower/Issues/blob/master/ChangeLog%202016.md).
