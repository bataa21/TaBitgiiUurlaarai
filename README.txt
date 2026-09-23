Та битгий уурлаарай — Web V2.0 Beta 3.2.1 — Launch Path Fix

Open index.html in a modern browser. No installation or internet connection is required.

Beta 1 gameplay foundation retained:
- one shared die that travels to the next player;
- Android-style guaranteed-six timing (3 misses when all pawns are home, otherwise 5);
- smarter tactical computer players;
- colored safe-cell and finishing-lane rings;
- Pisa Tower stacking on safe cells, oldest pawn at the bottom;
- existing plane, taxi, capture, exact-finish, bonus-roll, sound and mobile support retained.

Beta 2 Android Experience Pack:
- green ? help button with concise rules;
- three-page first-launch tutorial;
- new-game confirmation;
- automatic stable-turn saving and Continue Game prompt;
- stronger capture spin and balanced sound levels;
- small-device and large-text responsive safeguards.

Beta 3 Installable PWA Edition:
- approved Android dice-and-four-pawns icon;
- install support on Android, Windows and compatible browsers;
- offline play after the first hosted visit;
- standalone app mode with matching theme colors;
- automatic update detection and a visible Update button;
- winner statistics for rolls, captures, plane rides, taxi rides and duration.

Beta 3.1 fix:
- the service worker now ignores chrome-extension:// and other unsupported schemes;
- cross-origin browser-extension requests are never written to the game cache;
- cache identity bumped so GitHub Pages can activate the corrected worker.

Beta 3.2 identity protection:
- permanent manifest identity unique to this game;
- launch URL and app scope are explicitly limited to this deployed game folder;
- service-worker registration explicitly stays inside this game folder;
- the green APP badge appears only for this game's marked standalone launch,
  so a different PWA shell cannot be mistaken for this installed game.

PWA installation note:
The game must be opened through HTTPS (for example GitHub Pages) or localhost/WAMP.
Opening index.html directly still runs the game, but browsers do not allow service-worker installation from file:// pages.

Beta 3.2.1 launch-path fix:
- manifest ID, start URL and scope now resolve relative to the folder containing the game;
- this prevents an installed app from accidentally opening the GitHub Pages publisher root;
- the same package works from the GitHub repository folder and a localhost folder.

Important Edge note:
An already-installed PWA with a root scope such as / can still capture links before this page opens.
Beta 3.2 gives this game a separate permanent install identity, but it cannot change another app's scope.
If Plane Radar captures this URL, disable its supported-link handling, narrow Plane Radar's manifest scope,
or uninstall it while testing this game in a normal Edge tab.

The original uploaded web edition was not modified.
