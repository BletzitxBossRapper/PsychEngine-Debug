#

Code
Pull requests
More
Engine originally used on Mind Games mod

License
 Apache-2.0 license
 7 stars
 2k forks
 1 watching
 Activity
Public template repository · Forked from ShadowMario/FNF-PsychEngine
MaysLastPlaysThings/FNF-PsychEngine
 Branches
 Tags
This branch is 239 commits ahead of ShadowMario:main.
Latest commit
@MaysLastPlay10
MaysLastPlay10
…
3 days ago
Git stats
Files
README.md
Friday Night Funkin' - Psych Engine
Engine originally used on Mind Games Mod, intended to be a fix for the vanilla version's many issues while keeping the casual play aspect of it. Also aiming to be an easier alternative to newbie coders.

Installation:
You must have Haxe version 4.2.5, seriously, stop using older or newer versions, it won't work!

open up a Command Prompt/PowerShell or Terminal, type haxelib install hmm

after it finishes, simply type haxelib run hmm install in order to install all the needed libraries for Psych Engine!

If the compiler gives an error saying that hxCodec cannot be found read this issue to fix it: ShadowMario#12770

Customization:
if you wish to disable things like Lua Scripts or Video Cutscenes, you can read over to Project.xml

inside Project.xml, you will find several variables to customize Psych Engine to your liking

to start you off, disabling Videos should be simple, simply Delete the line "VIDEOS_ALLOWED" or comment it out by wrapping the line in XML-like comments, like this <!-- YOUR_LINE_HERE -->

same goes for Lua Scripts, comment out or delete the line with LUA_ALLOWED, this and other customization options are all available within the Project.xml file

Credits (+ Android Port Credits):
Shadow Mario - Programmer
RiverOaken - Artist
Yoshubs - Assistant Programmer
MaysLastPlay - Android Porter
Beihu235 - Second Android Porter
FutureDorito - Third Android Porter
Special Thanks (+ Android Special Thanks)
MA Jigsaw - Workflow and Android Things Creator
bbpanzu - Ex-Programmer
Yoshubs - New Input System
SqirraRNG - Crash Handler and Base code for Chart Editor's Waveform
KadeDev - Fixed some cool stuff on Chart Editor and other PRs
iFlicky - Composer of Psync and Tea Time, also made the Dialogue Sounds
PolybiusProxy - .MP4 Video Loader Library (hxCodec)
Keoiki - Note Splash Animations
Smokey - Sprite Atlas Support
Nebula the Zorua - LUA JIT Fork and some Lua reworks
Features
Attractive animated dialogue boxes:


Mod Support
Probably one of the main points of this engine, you can code in .lua files outside of the source code, making your own weeks without even messing with the source!
Comes with a Mod Organizing/Disabling Menu.
Atleast one change to every week:
Week 1:
New Dad Left sing sprite
Unused stage lights are now used
Dad Battle has a spotlight effect for the breakdown
Week 2:
Both BF and Skid & Pump does "Hey!" animations
Thunders does a quick light flash and zooms the camera in slightly
Added a quick transition/cutscene to Monster
Week 3:
BF does "Hey!" during Philly Nice
Blammed has a cool new colors flash during that sick part of the song
Week 4:
Better hair physics for Mom/Boyfriend (Maybe even slightly better than Week 7's 👀)
Henchmen die during all songs. Yeah :(
Week 5:
Bottom Boppers and GF does "Hey!" animations during Cocoa and Eggnog
On Winter Horrorland, GF bops her head slower in some parts of the song.
Week 6:
On Thorns, the HUD is hidden during the cutscene
Also there's the Background girls being spooky during the "Hey!" parts of the Instrumental
Cool new Chart Editor changes and countless bug fixes


You can now chart "Event" notes, which are bookmarks that trigger specific actions that usually were hardcoded on the vanilla version of the game.
Your song's BPM can now have decimal values
You can manually adjust a Note's strum time if you're really going for milisecond precision
You can change a note's type on the Editor, it comes with five example types:
Alt Animation: Forces an alt animation to play, useful for songs like Ugh/Stress
Hey: Forces a "Hey" animation instead of the base Sing animation, if Boyfriend hits this note, Girlfriend will do a "Hey!" too.
Hurt Notes: If Boyfriend hits this note, he plays a miss animation and loses some health.
GF Sing: Rather than the character hitting the note and singing, Girlfriend sings instead.
No Animation: Character just hits the note, no animation plays.
Multiple editors to assist you in making your own Mod
Screenshot_3

Working both for Source code modding and Downloaded builds!
Story mode menu rework:


Added a different BG to every song (less Tutorial)
All menu characters are now in individual spritesheets, makes modding it easier.
Credits menu
Screenshot_1

You can add a head icon, name, description and a Redirect link for when the player presses Enter while the item is currently selected.
Awards/Achievements
The engine comes with 16 example achievements that you can mess with and learn how it works (Check Achievements.hx and search for "checkForAchievement" on PlayState.hx)
Options menu:
You can change Note colors, Delay and Combo Offset, Controls and Preferences there.
On Preferences you can toggle Downscroll, Middlescroll, Anti-Aliasing, Framerate, Low Quality, Note Splashes, Flashing Lights, etc.
Other gameplay features:
When the enemy hits a note, their strum note also glows.
Lag doesn't impact the camera movement and player icon scaling anymore.
Some stuff based on Week 7's changes has been put in (Background colors on Freeplay, Note splashes)
You can reset your Score on Freeplay/Story Mode by pressing Reset button.
You can listen to a song or adjust Scroll Speed/Damage taken/etc. on Freeplay by pressing Space.
You can enable "Combo Stacking" in Gameplay Options. This causes the combo sprites to just be one sprite with an animation rather than sprites spawning each note hit. PsychEngine-Debug
Bitbox android PsychEngine 0.7.1
