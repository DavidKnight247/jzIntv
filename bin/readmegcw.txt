JzIntellivision Beta4.1, An Intellivision emulator by Joe Zbiciak

Ported to the GCW0 by David Knight due to a request by Dingoonity board members

All original artwork by Gab1975
Thanks to playtesters Ker, Gab1975 and Ghaleon
Fonts used are "Joy Circuit" by Ray Larabie and "ProggyTiny" by Tristan Grimmer

This version of JzIntv has been kindly provided by the original author and is of a more recent state than Beta4. Source code is packaged with the opk.
It is a complete re-porting and not based on versions of JzIntv previously released for the GCW0. 

The aim of the port was to use an updated version of the source-code, greatly improve rom compatibility and improve play experience with support for custom overlays.

I have modified the original authors code in the following ways:
Remapped controls
Enabled player 1/2 toggle
Enabled virtual numeric keypad with several user-defined settings in menu
Enabled user created overlays (place in $HOME/.jzintellivison/overlays folder)
Enabled menu
Autofix roms without cfg files (autogenerates missing .cfg file)
Autocreate directory structure
Triplebuffering
Created gcw0 makefile
Added manual
Added icon
Created opk

01/01/2015
Changed icon
Fixed Triple Challenge not working bug (please delete the Triple Challenge config file in .jzintellivison/cfgfiles if still not working)
Enabled virtual keyboard

HOW TO PLAY
You will need an intellivison bios rom set in order to play any games. These are legally obtainable from the Intellivision Lives! CD for Windows/Mac for example which also contains a selection of games. Place them in the $HOME/.jzintellivision/bios folder which autocreates on first run. The names of the bios files should be:

grom.bin
exec.bin

(and also optionally)
game.rom
ecs.bin <-needed to make use of the virtual keyboard

Game roms can be placed anywhere, the rom chooser will remember the last used rom location.

CUSTOM OVERLAYS
This version is unique as it supports user created custom overlays. The default numeric keypad is included. However for a more authentic experience it can be replaced by any png file with dimensions of 72x96. Each character therefore is 24x24. The png file must be labelled with the same name as the "recognised" game name with a .png extension. I have included the full list at the foot of this document.
e.g. for the game "Astrosmash" You would need to label your image either "Astrosmash.png" or "Astrosmash (DigiPlay).png"
and place it in the $HOME/.jzintellivision/overlays folder.
The recognised game name is printed in the output log so if you get stuck just read the log file, it will tell you what to do.

CONTROLS
A list of controls are available from the menu screen. Press SELECT at any time to view the controls.
"START" toggles between player 1 and player 2. An unobtrusive message will appear when you are using player 2 controls to avoid you being unaware however the default control setup is configured for player 1.

There are a couple of extra controls not listed on the controls menu. Pushing slider up will exit the current game back to the rom chooser menu. 
Pressing 'right shoulderpad + SELECT' will reset the current game.
Screenshots can be taken using the usual 'slider up + Y' combination.

David Knight
01/01/2015

Recognised game names follow:
"4-Tris"
"Keyboard Component 6502 EXEC"
"River Raid Prototype"
"Advanced Dungeon & Dragons Cloudy Mountain"
"Advanced Dungeon & Dragons Treasure of Tarmin"
"Adventure (Advanced Dungeon & Dragons prototype)"
"Adventures of TRON (Prototype)"
"Air Strike (Prototype)"
"Armor Battle (Slow Tanks)"
"Armor Battle (Fast Tanks)"
"Astrosmash"
"Astrosmash (DigiPlay)"
"Atlantis"
"Auto Racing (Real Steering)"
"Auto Racing (Intuitive Steering)"
"B-17 Bomber"
"Major League Baseball"
"Beamrider"
"Beauty and the Beast"
"Blockade Runner"
"Bomb Squad"
"Body Slam Super Pro Wrestling"
"PBA Bowling"
"Boxing"
"BurgerTime"
"Brickout (Prototype)"
"NBA Basketball"
"Bump 'N' Jump"
"Buzz Bombers"
"Space Cadet (Unreleased)"
"Carnival"
"Castle (Philly Classic Trailer)"
"Centipede"
"Checkers Rel. 1"
"Checkers Rel. 2"
"USCF Chess"
"Chip Shot Super Pro Golf (Caddy)"
"Chip Shot Super Pro Golf (Caddie)"
"Championship Tennis"
"Choplifter (Unreleased)"
"Crazy Clones (Prototype)"
"Congo Bongo"
"Commando"
"Deadly Dogs!"
"Super Pro Decathlon"
"Deep Pockets Super Pro Pool & Billiards (Unreleased)"
"Defender"
"Mattel Demonstration Cartridge"
"Mattel Demonstration Cartridge 1983"
"Demon Attack"
"Dig Dug"
"Diner"
"Donkey Kong"
"Donkey Kong Junior"
"Dracula"
"The Dreadnaught Factor"
"Dragonfire"
"The Dreadnaught Factor (Prototype)"
"Duncan's Thin Ice (Voochko hidden)"
"Easter Eggs.A (Prototype)"
"ECS BASIC ROM"
"The Empire Strikes Back"
"Master Component EXECutive ROM"
"Fathom"
"NFL Football"
"Frog Bog"
"Frogger"
"ABPA Backgammon"
"Go For The Gold (Unreleased)"
"Go For The Gold (Incomplete)"
"PGA Golf"
"PGA Golf (rerelease)"
"Grid Shock (Prototype)"
"Master Component Graphics ROM"
"Groovy!"
"Halloween Street (prototype)"
"Hard Hat (unreleased)"
"Masters of the Universe The Power of He-Man"
"NHL Hockey"
"Horse Racing"
"Hover Force 3-D (Unfinished)"
"Happy Trails"
"Hover Force"
"Hypnotic Lights"
"Ice Trek"
"Illusions"
"Jetson's Way With Words"
"Number Jumble"
"King of the Mountain"
"Kool-Aid Man"
"LadyBug"
"Land Battle"
"Spinning World"
"Lock 'n' Chase (6K variant)"
"Lock 'n' Chase (6K)"
"League of Light"
"Learning Fun I"
"Learning Fun II"
"Lock 'n' Chase (8K)"
"Loco-Motion"
"Math Fun (reverse entry)"
"Math Fun (forward entry)"
"Maze Demo"
"Maze-A-TRON"
"Microsurgeon"
"Melody Blaster"
"Astrosmash / Meteor"
"Mindstrike"
"Minotaur (Treasure of Tarmin prototype)"
"Mission-X"
"Motocross"
"Mousetrap"
"Mr. Basic Meets Bits 'n' Bytes"
"MTE-201 Test Cartridge"
"Stadium Mud Buggies"
"Nova Blast"
"Pac-Man (Atarisoft)"
"Pac-Man (INTV)"
"Pinball"
"Pitfall"
"Las Vegas Poker and Blackjack"
"Pole Position"
"Pong"
"Popeye"
"Quest (Unfinished)"
"QBert"
"Mattel Demonstration Cartridge (Revised)"
"Reversi"
"River Raid"
"Robot Rubble Prototype 1"
"Robot Rubble Prototype 2"
"Robot Rubble Prototype 3"
"Rocky and Bullwinkle"
"Roulette"
"Royal Dealer"
"Royal Dealer (Corrupt?)"
"Safecracker"
"Santa's Helper"
"Super NFL Football (Unreleased)"
"Scarfinger"
"Super Cobra"
"Scooby Doo's Maze Chase"
"Sea Battle"
"Sewer Sam"
"Shark! Shark!"
"Sharp Shot"
"Space Shuttle?"
"Mountain Madness Super Pro Skiing"
"U.S. Ski Team Skiing"
"Slam Dunk Super Pro Basketball"
"Slap Shot  Super Pro Hockey"
"Solar Sailer"
"Super Masters (Prototype)"
"Snafu"
"Super Soccer (Unfinished)"
"NASL Soccer"
"Killer Songs"
"Space Cunt (Ver 2)"
"Space Hawk"
"Space Armada"
"Space Battle"
"Space Spartans"
"Super Pro Football"
"Spiker! Super Pro Volleyball"
"Zzzz! Starring Spina the Bee"
"Night Stalker"
"Stampede"
"Star Strike"
"Sub Hunt"
"Swords and Serpents"
"Takeover"
"Tennis"
"Thin Ice"
"Thunder Castle"
"Tower of Doom"
"Triple Challenge"
"Triple Action"
"TRON Deadly Discs"
"Tropical Trouble"
"Truckin'"
"Turbo"
"Tutankhamun"
"Utopia"
"Vectron"
"Venture"
"World Championship Baseball"
"World Cup Soccer"
"White Water!"
"The Electric Company Word Fun"
"Worm Whomper"
"World Series Major League Baseball (Incomplete)"
"World Series Major League Baseball"
"Zaxxon"
"Space Patrol SDK-1600 Edition"
"Space Patrol Teaser Edition"
