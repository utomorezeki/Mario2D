Group 4

Each team member has two code reviews in the "Code Reviews" folder under Sprint 6. The group reflection and discussion on the Burndown Chart is in the "Burndown Chart Reflections" folder. The game is "Game.sln" and all related files are in the "Game1" folder.

New Feature 1: 
- Bat Mario: Rezeki Utomo
	added bat state mario and the item required to change mario into bat state. the bat state will only last for a couple seconds due to gameplay balancing. After the bat state is over, mario would turn back into the previous state he was before
	he entered the bat state. Research into random number generators were done in order to simulate the wind movement as the bat flies. This could clearly be seen when the bat is stationary or moving as it will shake up, down, and back independent
	of the user control. While in the bat state, mario is vulnerable despite the previous state he was in. If he got hit during bat state, he would die instantly. This is a design decision to prevent the game from being too easy. For testing purposes,
	the "y" key has been changed to turn mario into the bat state. During normal gameplay, mario has to pick up the powerup item hidden in boxes in order to turn into a bat.

New Feature 2:
- Rotating FireBeam Enemy type: By Dylan Guo

	A rotating firebeam consisting 3 diffent size fire balls spining around an used block serving as an new enemy type. This rotating firebeam can be added
at anywhere to create new hurdles for mario to progress. Any collision between mario and the each of the 3 fireballs will change the current mario state accordingly.
While the firebeam is rotating downward, the upward space is safe for mario to pass and vice versa.

New Feature 3:
- Infinite Level: Morgan Gongwer
	When game starts, player has the option to choode the normal 400 second game mode or the infinite mode where time does not decrease as it is infinite. The keys have been set to pressing N for normal and F for infinite. Three new classes had to be made in order to all this to function. A startScreen.cs was made to determine which key is pressed and then loads the appropriate level. InfiniteLevel.cs was made to house all the main updat, draw and aspects of the infinite level. Then InfiniteLevelLoader.cs was made to load the text files that create the infinite levels. Research was done on how to load multiple text files. Three booleans were made (begin, normal, infinite) to determine what state the game is in. If in normal, Mario starts with 3 lives and can gain, loose or completely die. When he is at 0 lives the game goes back to the beginning screen. If in infinite, when mario dies it goes back to the start screen. Pressing the R key while in normal or infinite mode will send you back to the game beginning.

New Feature 4:
- Shiny Patel


Keyboard Controls:
	Q - Quit Game
        W - Jump/Move Up
        A - Move Left
	S - Crouch/Move Down
	D - Move Right
	Z - Jump/Move Up
	X - Shoot Fireballs in Fire Mario State
	C - Invisible Block to Used Block
	Y - Bat State
	U - Large Mario State
	I - Fire Mario State
	O - Dead Mario State
	N - Normal Mode
	F - Infinite Mode
	P - Pause
	R - Reset to Start Screen and all Levels
	Up Arrow - Jump/Move Up
	Down Arrow - Crouch/Move Down
	Left Arrow - Move Left
	Right Arrow -  Move Right
	Space - Jump


GamePad Controls:
	Left Thumbstick Up - Move Up
	Left Thumbstick Left - Move Left
	Left Thumbstick Down - Crouch/Move Down
	Left Thumbstick Right - Move Right
	A Button - Jump
	B Button - Shoot Fireballs in Fire Mario State


***We ran Code Analysis and received 0 errors and 0 warnings. Below is the output:
	1>------ Rebuild All started: Project: Game, Configuration: Debug x86 ------
1>  Game -> C:\Users\Admin\Source\Repos\Mario4.02\Game1\bin\Windows\x86\Debug\Game1.exe
1>  Running Code Analysis...
1>  Code Analysis Complete -- 0 error(s), 0 warning(s)
========== Rebuild All: 1 succeeded, 0 failed, 0 skipped ==========


New Feature 2:
- Rotating FireBeam Enemy type: By Dylan Guo

	A rotating firebeam consisting 3 diffent size fire balls spining around an used block serving as an new enemy type. This rotating firebeam can be added
at anywhere to create new hurdles for mario to progress. Any collision between mario and the each of the 3 fireballs will change the current mario state accordingly.
While the firebeam is rotating downward, the upward space is safe for mario to pass and vice versa.


New Feature 3:
PiranhaPlant Enemy type: By Shiny Patel

- Added piranha plant to level 1. The game automatically draws a piranha plant for every 
"standardPipe" in the .csv file. 
- The piranha plant emerges from and submerges into the pipe. There is a short interval between the 
two during which it is safe for Mario to stand on the pipe.
- When Mario collides with piranha plant, appropriate Mario state change takes place. 
- A piranha plant can only be killed by a fireball from the fire Mario.
