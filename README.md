# connect-4

A multiplayer Connect-4 game implemented exclusively with git.

## How to use
* copy all the git aliases from ``aliases.txt`` into your own global git config (``git config --global -e``)
* create a local folder, copy its path -> ``git c4i "[local_folder]"``
* choose a username -> ``git c4r [username]``
* if necessary get authorization for this git repo

## Commands
* c4h (help): print all c4 commands
* c4n (new): start new game
  * 1st argument -> 1 for starting player, 2 for other player
  * 2nd argument -> username of opponent
* c4l (load): load game and print current board state
  * with match ID -> load a specific game
  * without match ID -> load current / most recent game
* c4s (status): list your current games amd user information
* c4m (move): make move (1-7)
  * with additional argument -> sends a message to your opponent
* c4u (undo), c4f (forward): move forward or backward (you can't actually undo any moves, it's meant to be used as a history mode / spectating only)
* c4r (register): register / login with username
  * if user already exists -> login
  * if user doesn't exist -> register + login
  * usernames must not contain a comma
* c4p (print): print leaderboard
* c4i (install): clones and registers path for local copy of git repo

## Notes
* there is no authentication / security, users are required to be honest and use only their own usernames and the git aliases as the only interface
* do not interact with this repository in any other way
