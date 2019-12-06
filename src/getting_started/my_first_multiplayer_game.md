---
name: My First Multiplayer Game
categories:
    - Tutorial
---

# My First Multiplayer Game

!!! warning
    Flagged for Review.
    Incomplete or outdated information may be present.

## Overview

Welcome to CORE! We're excited to have you in Closed Alpha and can't wait to see what you create. To get you started, we're going to walk you through creating your first multiplayer game in CORE... in 10 minutes!

* **Completion Time:** 10 minutes
* **Knowledge Level:** Beginner! No experience necessary!
* **Skills you will learn:**
    * Editor Basics
    * CORE Content (Props & Materials)
    * Player Movement Settings
    * Community Content
    * Publishing

## Create a New Game

To get started, we're going to create a new project.

1. Click on **Create New**.

   ![Create New](../img/EditorManual/MyFirstMultiplayer/CreateNew.png){: .center}

2. Select the **Deathmatch** framework!

   ![Deathmatch](../img/EditorManual/MyFirstMultiplayer/Deathmatch.png){: .center}

3. Name your project `MyFirstMultiplayerGame` or whatever you like! Then, click Create.

   ![Name](../img/EditorManual/MyFirstMultiplayer/MyFirstMultiplayerGame.png){: .center}

### Explore the Map

The Deathmatch framework gives a great starting point! Let's try it out ourselves.

1. Behold the magnificence of this whiteboxed, free-for-all game framework! Let's jump in by pressing **Play**.

   ![Whitebox](../img/EditorManual/MyFirstMultiplayer/WhiteboxMapMarked.png){: .center}

2. Out of the box, you have a character who can move and jump! Explore the map by moving your character with the <kbd>WASD</kbd> keys and jumping with <kbd>Space</kbd>. Shoot the default gun with your left mouse click and interact with the door with <kbd>F</kbd>.

   ![PlayMode](../img/EditorManual/MyFirstMultiplayer/PlayMode.png){: .center}

3. But we're all by ourselves. 😞 That's no fun, so let's test out the multiplayer experience by simulating two clients! Near the pause button, click on the **Multiplayer Preview Mode** button and select 2 Players.

   ![TwoPlayers](../img/EditorManual/MyFirstMultiplayer/TwoPlayers.png){: .center}

4. Let's press Play again! Two clients will launch now. You control whichever character is in your current active window.

   ![MPPreview](../img/EditorManual/MyFirstMultiplayer/MultiplayerPreviewPlay.png){: .center}

!!! tip
    Note that you can use <kbd>Alt</kbd> + <kbd>Enter</kbd> to toggle between fullscreen and windowed mode. You can also use <kbd>Win</kbd> + <kbd>Arrow</kbd> to dock the screens side by side like above!

## Make It Your Own

So we have a whiteboxed map, and that's great and important in testing design! Now, let's customize the map now and make it our own.

1. Navigate to the **CORE Content** window. You have access to a massive library of 3D assets, materials, and more for your game creation in CORE!

   ![Add Props](../img/EditorManual/MyFirstMultiplayer/AddPropsMarked.png){: .center}

!!! note
    If you can't find the "CORE Content" window or accidentally close it, you can reopen the window by going to View > Core Content in the toolbar at the top of the editor.

2. Click on "3D Objects" and then drag and drop props into the editor viewport! In this example, we're going to place some bushes.

   ![DragDrop](../img/EditorManual/MyFirstMultiplayer/DragDropBushes.gif){: .center}

3. You can move, rotate, and scale all these objects! `W` activates Translation Mode to move objects; `E` activates Rotation mode; and `R` activates Scale Mode to resize objects. Let's try click on an arrow and dragging an object along an axis.

   ![Move](../img/EditorManual/MyFirstMultiplayer/MoveBushes.gif){: .center}

4. Press Play. Currently, if you try to move through a bush, you'll be stopped once you collide with the object.

   ![Stuck](../img/EditorManual/MyFirstMultiplayer/StuckInBushes.png){: .center}

5. Bushes are great as environmental props to hide players, but it'd be great to let players push past them to surprise enemies in this game! Let's click on a Bush and check out the Properties window. By default, this Bush is "Collideable" but with a simple click, we can turn that off.

   ![Collison](../img/EditorManual/MyFirstMultiplayer/NoCollisonBush.gif){: .center}

!!! note
    If you can't find the "Properties" window or accidentally close it, you can reopen the window by going to View > Properties in the toolbar at the top of the editor.

### Designing Your Level

Let's take this time to build out our own game! We're going to apply materials to whiteboxed scene, add more props, and add a sky to finish off the scenery.

1. Let's check out the Materials library within **CORE Content**! It's fast and easy to drag and drop any material onto an object to apply it.

    ![WallObjects](../img/EditorManual/MyFirstMultiplayer/MaterialExample.gif){: .center}

2. But there's a really fast way to apply materials to all the objects in our game! To the right of the editor, game objects are listed in the "Hierarchy." Let's use the search bar to find all the "Wall" objects. Then, click the "Select" button to the right.

    ![WallObjects](../img/EditorManual/MyFirstMultiplayer/SelectWalls.gif){: .center}

3. Search for "Bark Oak 01" (or choose any material you like!) and drag it back into the hierarchy where all the selected walls are currently highlighted.

    ![WallObjects](../img/EditorManual/MyFirstMultiplayer/WoodWalls.gif){: .center}

4. Looking good! Let's practice some more. Try searching the Hierarchy for "windows", using the Select button, and applying the same material.

    ![WoodLevel](../img/EditorManual/MyFirstMultiplayer/WoodLevel.png){: .center}

5. Let's switch out this whitebox floor! Search the hierarchy for "floor", use the "Select" button to select all floor pieces, and drag and drop the material "Grass Clumps" onto the selected floor.

   ![WoodFloor](../img/EditorManual/MyFirstMultiplayer/WoodFloor.png){: .center}

6. Now, it's your turn! Apply a material to the stairs and add more props to your game! Remember you can scale, rotate, and transform objects as well as explore an object's Properties!

   ![FinishArt](../img/EditorManual/MyFirstMultiplayer/FinishArt.png){: .center}

!!! info "How do I make my own material?"
    If you want to learn more about customizing materials, check out our [Custom Material tutorial](../tutorials/art/custom_materials.md).

7. Awesome! This scene looks rather dark though. Let's make it more vibrant with some better lighting! In "Core Content," search for sky. Then, drag and drop "Sky Whimsical Sunny Saturation."

   ![VibrantLevel](../img/EditorManual/MyFirstMultiplayer/VibrantLevel.png){: .center}

!!! tip
    In CORE, you even have tons of customizeable post process effects and VFX. Search for "Advanced Bloom Post Process" in CORE Content and try it out!

### Customizing the Gameplay

The map's in good shape now! Let's change up the gameplay itself now. There are lot of props on the map now, so let's give the player more power to hop over them.

1. Find the "Player Settings" in the "Game Settings" folder or search the Hierarchy for it.

   ![PlayerSettings](../img/EditorManual/MyFirstMultiplayer/PlayerSettings.png){: .center}

2. In the Properties window of "Player Settings," change the Jump Max Count to 2 so all players have a double jump! Press Play and try it out with <kbd>Space</kbd>.

   ![DoubleJump](../img/EditorManual/MyFirstMultiplayer/DoubleJump.png){: .center}

3. Great! Now, let's make this game have shorter rounds since 10 Kills may take a while. Let's go into the "Gameplay Settings" folder and select "Round Kill Limit."

   ![RoundKillLimit](../img/EditorManual/MyFirstMultiplayer/RoundKillLimit.png){: .center}

4. In the Properties window, change the "KillLimit" custom property to 3. Now, if you playtest, the winner will be whoever gets 3 kills first!

   ![ChangedKillLimit](../img/EditorManual/MyFirstMultiplayer/ChangedKillLimit.png){: .center}

5. To match that game logic, let's change the UI text to match the Round Kill Limit. In "UI Seetings", find "Game Instructions" and click on the "UI Text Box." In Properties, change the Text field to 3.

   ![ChangedGameInstructions](../img/EditorManual/MyFirstMultiplayer/ChangedGameInstructions.png){: .center}

6. Let's move the "Player Start" where players spawn to be further apart. Press `V` to toggle gizmo visibility-- you can now see the camera, spawn points, and trigger boxes.

   ![PlayerSpawn](../img/EditorManual/MyFirstMultiplayer/PlayerSpawn.png){: .center}

!!! tip
    With the shortcut key `0`, you can create a spawn point at your cursor's location. Check out more editor shortcuts [here](../editor_keybindings.md)!

### Choose Your Weapon! from Community Content

1. Navigate to **Community Content**, where creators can publish and share their creations with the community! Let's search for a weapon and then click on the `Import` button to download the template into your local project. In this example, the "Tree Gun" will be imported.

   ![CCSearch](../img/EditorManual/MyFirstMultiplayer/CCSearch.png){: .center}

!!! note
    If you can't find the "Community Content" window or accidentally close it, you can reopen the window by going to View > Community Content in the toolbar at the top of the editor.

2. Now, in the "Gameplay Settings" folder in the hierarchy, locate the "Starting Weapon" folder. In the custom property called "EquipmentTemplate", drag and drop your imported gun's template. The imported weapon can be found under **CORE Content** in the "Imported" category.

   ![StartingWeapon](../img/EditorManual/MyFirstMultiplayer/StartingWeapon.png){: .center}

3. Press Play and test our your awesome new gun!

!!! info "How do I make my own weapon?"
    It's easy! Check out our [Basic Weapons Tutorial](../tutorials/gameplay/weapons.md).

### Publishing Your Game

Flow is still in progress on the engine side.

(Show Final Website)

### Next Steps

Now's the best part! Playtesting with friends!
Engage with community in #playtest in :fab fa-discord: [Discord](https://discordapp.com/invite/3H4j3YJ).

Post a screenshot of character/map/playtest in #showcase in Discord.
You're doing amazing!! Supportive encouragement here.

Excited? Check out these tutorials next:

* Intro to Enviro Art (Terrain)
* Weapons (Gun)
* Abilities (Dodgeroll)