# dungeons-4

### general improvements
- when right-cllicking to move or attack, all of the units pause for a moment (presumably to recalculate the pathing). if I spam clicks like SC2 players do, the units take considerably longer to get to their destination, and look like spazzes. there should be no pause, and the units should just go the new direction
	- when clicking in roughly the sane spot, only the last nodes of the path should need to be recalculated
- ability to set the floor tile of a dig tile:
	- dig tiles have a blue outline to them. floor tiles have a blue/yellow color to them (depending on if I have the gold). if I drag the floor tiles over the dig tiles (it should turn blue with the floor tile I set), the snot should dig out the tile, then if I don't have the gold, it'll turn yellow and he'll keep digging. however, if I have the gold, immediately after digging, he'll place the floor tile.
- ability to set floor tiles directly on unexcavated tiles, which the snot will dig out, then put the floor down (same as above but in one step)
- when selecting the mission, show which difficulty level the mission have been beat on (maybe put a glow or border around the difficulties that it's been beat on?) (see dungeon run section below).

### wishlist
- ability to pause constrution. often times I queue up a number of traps to be built, but then that means that I cannot do any research until all of the traps are built, cause every time I get enough gold for the next trap, it spends it. the only way to get them to stop building, is to cancel all of the yellow traps, but then I have to re-place them again later, which is annoying
- ability to a-move (say by holding ctrl or something).
	- when a-moving a click on the ground, any enemy unit gets within shooting/hitting range on thier way to destination, it will engage the enemy until the enemy unit has left some range amount (probably a little more than weapon range), and after having left the range, it'll continue on to the path toward the destination.
	- when a-moving a click on a unit, the unit will path toward the unit clicked on, attacking anyone along the way that gets in range of each unit (they pause for a second to shoot/swing before continuing on)
		- for example, I ctrl-click to attack the priestess in the back of the group with my gazers: right now, they go straight toward her, often passing swordsmen along the way. I want them to shoot the swordsmen on the way to getting in range of the priestess. to simulate the same thing requires a lot of micro: click on the priestess, wait 0.5s, press X (stop), wait for them to shoot, press the priestess again (and repeat)
	- it'd also be a nice touch if the line and arrows drawn are red (attack) instead of green (move)

### dungeon run
- it's weird that a game called "dungeons" doesn't have a dungeon run mode. if the the statistics for each mission (subtracting the cutscene time) were saved, then each mission can be looked at like a dungeon run.
- add more randomisation to the levels, giving different bonuses depending on random powerup discoveries in the underworld.
	- this adds the dynamic of wanting to get evilness in overworld, or excavating the dungeon to possibly get a really great boon
- also, this would be really cool with coop mode. -- which I haven't tried yet, so I can't say much more.
