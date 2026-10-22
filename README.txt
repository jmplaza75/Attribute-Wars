ATTRIBUTE WARS 1.0
A ZX SPECTRUM 48K GAME
CREATED BY JOSE MANUEL PLAZA

Release Candidate 1

Copyright (c) 2026 Jose Manuel Plaza
Licensed under the MIT License. See LICENSE for details.

ABOUT THE GAME
--------------
Attribute Wars is a color arcade game for the ZX Spectrum 48K.

Move the cursor over an 8x8 board and paint tiles to create temporary
barriers. Paint enough tiles to complete the level while avoiding the enemy.
Each scenario has its own map and enemy behavior:

  THE GRID    The hunter follows the shortest path and tries to intercept you.
  THE MAZE    The patrol follows a route and pursues you when you get close.
  THE SIEGE   The destroyer follows you and breaks the barriers in its way.

There are 99 levels. Every three levels the scenario changes and the objective
grows. The enemy speed has a minimum cadence, so the game remains playable as
the level counter increases.

LOADING
-------
1. Start a ZX Spectrum 48K emulator, such as Fuse.
2. Load AttributeWars-1.0.z80 as a snapshot.
3. The title screen appears. Press SPACE to start.

The snapshot uses ZX Spectrum 48K RAM, PC $8000, SP $FF00, interrupt mode 1
and no compression.

CONTROLS
--------
Q       Move up
A       Move down
O       Move left
P       Move right
SPACE   Paint the current tile / confirm / return

On the title screen:
I       Instructions
C       Credits
SPACE   Start a new game

GAME RULES
----------
- Paint the required number of tiles to complete the level.
- A newly painted tile becomes a temporary green barrier.
- Barriers expire after 400 frames and turn cyan.
- You have up to 5 paint charges. One charge is restored every 100 frames.
- White walls are permanent and cannot be painted.
- You have 3 lives. A life is lost when the enemy reaches you.
- After losing a life you are invulnerable for 100 frames.
- You earn 10 points for each new tile and 100 bonus points per completed
  level.
- You earn one extra life for each 1,000 points, up to a maximum of 5 lives.
- The score is limited to 65,530 points.
- The high score is kept for the current session only.
- GAME OVER returns to the title with a new SPACE press. Release the key and
  press it again to start.

PACKAGE CONTENTS
----------------
AttributeWars-1.0.z80
README.txt
CONTROLS.txt
CHANGELOG.txt
LICENSE
SHA256SUMS.txt

VERIFYING THE DOWNLOAD
----------------------
The SHA256SUMS.txt file contains the SHA-256 digest of every other file in
this package. From the directory containing the files:

  sha256sum -c SHA256SUMS.txt

On macOS:

  shasum -a 256 -c SHA256SUMS.txt
