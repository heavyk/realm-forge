# dungeons-4

### general improvements
- when right-cllicking to move or attack, all of the units pause for a moment (presumably to recalculate the pathing). if I spam clicks like SC2 players do, the units take considerably longer to get to their destination, and look like spazzes. there should be no pause, and the units should just go the new direction
	- when clicking in roughly the sane spot, only the last nodes of the path should need to be recalculated
- ability to set the floor tile of a dig tile:
	- dig tiles have a blue outline to them. floor tiles have a blue/yellow color to them (depending on if I have the gold). if I drag the floor tiles over the dig tiles (it should turn blue with the floor tile I set), the snot should dig out the tile, then if I don't have the gold, it'll turn yellow and he'll keep digging. however, if I have the gold, immediately after digging, he'll place the floor tile.
- ability to set floor tiles directly on unexcavated tiles, which the snot will dig out, then put the floor down (same as above but in one step)
- when selecting the mission, show which difficulty level the mission have been beat on (maybe put a glow or border around the difficulties that it's been beat on?) (see dungeon run section below).
- ability to scroll the credits with the finger/mouse (like in ... forgot)
- in mission select sreen, add ability to click on the buff to deactivate it

### wishlist
- ability to pause constrution. often times I queue up a number of traps to be built, but then that means that I cannot do any research until all of the traps are built, cause every time I get enough gold for the next trap, it spends it. the only way to get them to stop building, is to cancel all of the yellow traps, but then I have to re-place them again later, which is annoying
- ability to a-move (say by holding ctrl or something).
	- when a-moving a click on the ground, any enemy unit gets within shooting/hitting range on thier way to destination, it will engage the enemy until the enemy unit has left some range amount (probably a little more than weapon range), and after having left the range, it'll continue on to the path toward the destination.
	- when a-moving a click on a unit, the unit will path toward the unit clicked on, attacking anyone along the way that gets in range of each unit (they pause for a second to shoot/swing before continuing on)
		- for example, I ctrl-click to attack the priestess in the back of the group with my gazers: right now, they go straight toward her, often passing swordsmen along the way. I want them to shoot the swordsmen on the way to getting in range of the priestess. to simulate the same thing requires a lot of micro: click on the priestess, wait 0.5s, press X (stop), wait for them to shoot, press the priestess again (and repeat)
	- it'd also be a nice touch if the line and arrows drawn are red (attack) instead of green (move)
- ability to switch dungeon/overworld left/right

### dungeon run
- it's weird that a game called "dungeons" doesn't have a dungeon run mode. if the the statistics for each mission (subtracting the cutscene time) were saved, then each mission can be looked at like a dungeon run.
- add more randomisation to the levels, giving different bonuses depending on random powerup discoveries in the underworld.
	- this adds the dynamic of wanting to get evilness in overworld, or excavating the dungeon to possibly get a really great boon
- also, this would be really cool with coop mode. -- which I haven't tried yet, so I can't say much more.
- other/different/alternate narrative storylines can be created
	- updating dungeons 3 story, or any of the many DLCs
	- I personally like the idea that there's a narrative foundation to a dungeon run
	- also, with the addition of the level editor, and existing multitude of props, models, and voicelines, it's (eventually, lol) possible for custom dungeon narratives/runs to be created and shared

### stuff
- way to tell snots to automatically add batteries to work units
- coi-style camera
- (idle / available / total) snots
- in dungeon, ability to toggle between overworld/tactical mode and hand of terror

### bugs?
- if I have a pylon of might building, it will block all demons from resurrecting, until the pylon is built. I would expect demon resurrection to be higher priority. right now, the only way around it is to delete the pylon.
- build a torture chamber, then build a torture apparatus, then before it's built, delete it; it'll delete the floor tile underneith as well as the apparatus. none of the other buildings exhibit this behaviour.

### 2024-01-29 01:05 - fun thought experiment: narrator without a voice

for a moment, I just want to try playing dungeons-4 without a narrator's voice. I know that this would change the perspective from ironic comedy to a fantasy drama, but the idea is that instead of the narrator giving voice commands, instead absolute-evil has to direct everything with noise responces to the user's play style.
to do this, the first thing that needs to change is the way that the music system reacts to the player, instead of directs the player. the music should tell the narrative of what "should happen" instead of what "is happening". to do this, I will consider that there are some quantity of loops of (10-30s) which describe a different aspect of an emotion. the emotion itself is what is playing, but different aspects give the musical narrative texture. instead of combat vs peace, these should be imagined something like an opera where there are characters playing out a scene, and each scene is one loop. variations on the scene are part of the detail of the loop, and even though it could be a complex scene, the emotion that scene conveys, can usually be summarized into 1-5 words or so; those are the category of the music and so what the player is listening to sounds really awesome because it's a full opera playing in the background.
	recently, after playing dungeons-4, I did some research into mozart and beethoven. in a number of his things, he's telling a story with the music. other great examples of this is handel's "triumph of time y el desengano" -- engano is fraud, so desengano is to remove the fraud (the unfrauding -- or dis-illusionment). the other is "magic flute" by mozart, and "creatures of prometheus" by beethoven. each "act" or is separated into movements or scenes (depending on how visual it is), and so I consider each of those to be a *loop* or a *stint*.
opposite to the *loops*, which start at about the same place they end, a *stint* however ends in a different place than it starts. we can imagine the starting and ending point of each loop/stint to have a number of quaternians (or a vector with a magnitude), and it just looks for a starting place that ends roughly (within some range based on parameters) where it ends. those can be thought of as transitions, and each vector/quat is just descriing things like the drums, visual or sensory descriptiopns (wind, rain, sun, hot), and temporal descriptions (night/day, spring/summer/fall/winter), or environments (clubs, boats, beach). then, a "composition" becomes just a series of transitions from one set of descriptions to another, (optionally) accompanied with a script or narration of the scene -- which are also descriptions.
visual cues can be given to the player instead of verbal commands (as long as they're easy to remove/add/customize).
verbal narration can also take advantage of this style of transitioning, if the narrator is described in terms of these directions (quaternian/vector) as well
