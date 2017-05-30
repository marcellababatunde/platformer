# Pygame Platformer

## About
<img src="/nog2k17.png" width="360">

## Ideas for student projects

### Easy

- Name your game.
- Change the dimensions of the game window.
- Find your own custom artwork for blocks.
- Find your own custom artwork for the hero.
- Find your own custom artwork for enemies.
- Find your own fonts.
- Find your own sound effects and music.
- Customize the background layer for a level.
- Customize the scenery layer for a level.
- Create a custom splash screen.
- Improve the display_message function so that the text is in a box making it easier to read against the background.
- Change point value for coins.
- Make power-ups give points to the player.
- Display hearts/max rather than just hearts.
- Update the display_stats function so that it shows the name of the current level.
- Add a victory sound that plays when the game is won.

### Medium

- Let the 'S' key toggle sound on and off. Show a little speaker/mute icon to indicate the current state of sound.
- Let the 'M' key toggle music on and off. Show a little note icon (crossed out or uncrossed) to indicate the current state of music.
- Create your own custom artwork. http://www.piskelapp.com/ is a good site for this.
- Create invincibility (star) power-up. (The optional arguments on the play_sound function can help you match an invincibility sound length to the invincibility period.)
- Increase the max hearts a player can have when some milestone is achieved.
- Add prizes other than coins and give them a point value.
- Track coins separately from the score. (They can still be worth points.) Give an extra life when a number of coins is earned. Reset the coin count after a life is given.
- Invent your own power-up which lasts a limited amount of time or until the player hits an enemy.
- Invent a "power-up" which has a negative consequence on a player other than reducing hearts or lives.
- Display lives with a character icon x number of lives.
- Put gaps in the blocks that run along the bottom of the level. Then make a player die when they fall through the bottom of the world. You'll need to make sure enemies that fall through are also removed from the game. Pygame's sprite.kill() function will be useful for this.
- Make a credits screen for when the player wins the game.
- Add a 'Pause' stage to the game which is activated when the player presses 'P' (or a button on the joystick). All movement and time should stop during a pause stage. Pressing 'P' again should resume. Be sure to show a message indicating the game is paused.
- Give points for getting the flag at the end of the level. Do so in a way that landing higher on the flagpole earns more points.


### Hard

- Design a complex standard level.
- Incorporate different kinds of levels (normal, space level, underwater, etc.) into the game.
- Change the game so that it uses the XBox controller instead of the keyboard. (https://github.com/joncoop/pygame-xbox360controller)
- Kill enemies when you land on them. You'll need to check which direction you hit the enemy from in process enemies. Award different point values for different enemy types.
- Make the game save high scores to a text file in a data folder.
- Create some other kind of custom enemy with unique behavior.
- Display actual hearts to show health. Show empty hearts when health is not full.
- Show time on the stats layer. Give a time bonus for completing a level. Have the hero die if the level is not completed in a set amount of time.
- Animate a background element such as clouds or flickering torches. (This is probably best accomplished by creating another layer that scrolls along with the background or scenery layer rather than trying to blit directly on one of those layers.)
- Add secret parts of the level that utilize vertical scrolling.

### How clever are you?
- Add ladders to the game. If a player is on a ladder, don't apply gravity. Assign vy by player input instead. Also disable jumping while on a ladder. You should use animated climbing images too.
- Put switches in the game that open and close areas of a level.
- Create a Chest object with a boolean attribute locked set to True when it is initialized. Then create a Key object. If the player intersects a locked chest with a key, then locked should be set to False and the image should be updated. Spawn a prize that the player can acquire in the grid location directly above the chest when it is unlocked. Be sure to take away the players key when the character respawns after dying or at the start of a new level.
- Give your player a gun. Let your player kill enemies by shooting them. You'll need to create Bullet objects which spawn at the hero's gun and travel in the direction the hero is facing. Bullets shouldn't travel indefinitely. Limit the number of ticks a bullet will exist before it calls the kill() function on itself. Enemies can be given a process_bullets function. (You might need to make the shooter/hero a bullet parameter so that when the bullet hits an enemy, points can be awarded.)
- Make a sign you can read or a character that 'speaks'. Display a message when the hero intersects the sign or speaking character while holding the up arrow. Don't use the default display_message function. Put a function in the Sign/SpeakingCharacter class that makes a popup that looks like text on a sign or perhaps a speech bubble.

### More!

- Create a text/image advertisement for your game.
- Create a video advertisement for your game.
- Create a website for your game using GitHub Pages.
- Write a review of a classmate's game. Include screenshots.
- Create a video review of a classmate's game.

## Grading

Each small phase of the game we've built in class will count as a minor assessment. (You'll get a 100% for each unless I suspect that you're not keeping up. In that case, I'll check up on you individually.)

One major assessment will be to create a single level of a game with custom artwork, complex level design, and a couple selected easy/medium features.

The second major assessment will be customizing the game by adding a variety of easy, medium, hard features, each of which has different point values.
