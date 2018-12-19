# relog
Forked from wuaw's [relog](https://github.com/wuaw/relog) module. Added a few extra features for convenience.
(Fixed !relog number and !relog nx)

### Dependencies
Converted to Pinkie Pie's [command](https://github.com/pinkipi/command) module. If you don't have it, just get it, seriously.

Requires the definition for `C_CHANGE_USER_LOBBY_SLOT_ID` to prevent one of the commands from bugging out if you reorder your character list. I've included it in this repository, so copy it to your `tera-data/protocol` folder.

### Usage
`!relog name` in chat, then don't touch anything until the module logs in for you

`!relog number` type in a number to relog to the n-th character from your selection list.

`!relog nx` type in nx (literally) to relog to the next character in your list.

### Known Issues
If your character gets hit within 10 seconds of using `!relog`, the client and server state will be desynced and you will have to restart client.

If you use `!relog` while dead, the client will crash.

Can possibly reposition characters?

!relog nx can sometimes not log to the next character???
