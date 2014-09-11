Issues
======

_**Note:** Everyone on Windows Vista or higher should read [this](https://github.com/Windower/Issues/wiki/Enabling-automatic-crash-dumps) and follow the instructions there, regardless of whether an error is happening already or not.

This is Windower's public issue tracker. If you're experiencing any bugs with Windower, feel free to report them here. Below are a few guidelines for bug reporting that will help both you and us in faster debugging, so please read them and try to follow them.

Before posting please make sure of two things.

1. That this is actually a Windower error. See if it's happening without Windower as well. If it does, there is unfortunately very little we can do for you. The best general info is to run a file check, and see if some corruption occurred at some point, and if that doesn't help, consult various forums to see if other people have experienced it and may be able to provide a solution. If not, you'll have to file a bug report with SE and possibly contact their tech support to get it resolved.
2. Make sure it hasn't been posted already. At the top of this page there is a search bar which can be used to search the entire repository. If you think you found the same error with a slightly different experience or circumstance post in that thread regardless and provide additional information, which will make it easier for us to eventually find the bug.

If neither of the above applies, here's a quick rundown of how and where to report issues:

* ***Unintended behavior*** (including simply not working), **non-crashing errors** or a ***feature request***
  - **Addon:**  
    Report it on the *addon developer's* issue tracker. The Windower launcher provides a link with the correct tracker for each addon. Be specific with what you think is incorrect or what you'd like to have incorporated.
  - **Plugin** or **Windower**:  
    Report it on [this issue tracker](https://github.com/Windower/Issues/issues). As above, be specific with what you think is incorrect or what you'd like to have incorporated.
* ***Crash***
  - **Plugin**:  
    Report it on [this issue tracker](https://github.com/Windower/Issues/issues). Provide as much information as possible. When a plugin crashes, the console will tell you why. A typical error message may look like this:  
    `PluginName encountered a fatal error and must be terminated. Error: Access Violation in IncomingChunk method.`  
    When reporting a plugin crash *always* provide the type of the error (in this case an *Access Violation*) and where the error occurred (in this case *IncomingChunk*). Also make sure you give us as much information as possbile about *how* you encountered the error, i.e. what you were doing, what event you were in, if you were performing an action or being passive, etc. as well as your current setup (which plugins and addons you were using, any configuration you think may be relevant or any other third party tools you think might have been interfering).  
    In addition to that, please see if you can replicate the error, and if so, tell us exactly how. It's very hard to debug somethng we cannot experience ourselves, which is the reason for most of the currently opened issues still being open.
  - **POL**:  
    POL crashing indicates a serious low-level error in one of our plugins or the Hook. If that happens, you won't get a detailed error message, but you should still try to give us as much information as possible (where were you, what were you doing, your setup, etc.).  
    If you are able to replicate the issue, you can [make a crash dump](https://github.com/Windower/Issues/wiki/Enabling-automatic-crash-dumps) and upload it so we can take a look at it. This is the best way to get it resolved. Make sure you actually upload the `.dmp` file, as just some copy/pasted crash information will tell us very little about the error.
