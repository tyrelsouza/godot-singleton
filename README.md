# Sample of a Singleton using autoload in Godot

Sample proof of https://docs.godotengine.org/en/stable/tutorials/scripting/singletons_autoload.html

This project shows how to use a Singleton script `game_state.gd`

The script loads once, and prints "Game State Ready".

Then loads `main.tscn` which `main.gd` prints "main".

Then in main's ready, it just changes to `not-main.tscn`.

At which point, "Game State Ready" does NOT print again, to show that it's only loaded once.

"not main" then prints, from the `not_main.gd` ready function.

