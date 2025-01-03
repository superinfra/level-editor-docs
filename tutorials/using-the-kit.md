# Intro
This tutorial explains how to use the kit and the optional plugin. **Watch the video on [the Tutorials page](/tutorials) to learn how to use Roblox Studio.**

|Using the Kit            |          
|-------------------------|
|Steps: **3**             |
|Skill level: **Beginner**|
|Length: **~10 min.**     |

# 1. Getting the kit (2 min.)
Welcome to the tutorial! First, you should download the kit. Not much you can do without it, huh? You can do that in two ways:

* Download the .rbxl file directly:
	1. Go [here](/downloads/kit.rbxl) to download the file.
 	2. Open up a new file in Studio, or [use a template](/templates). (`Ctrl+N` or `Cmd+N` for Mac)
  3. Right-click the Workspace in the Explorer window (View tab > Explorer) and select `Insert From File`.
  4. Select `kit.rbxl` from the file explorer that appears.
  5. With the kit selected, run this code in the command bar (View > Command Bar, look at the bottom of the screen):
  ```lua
	local kit = game.Selection:Get()[1]
 	kit.Blocks.Parent = game.ReplicatedStorage
 	kit.LevelNameHere.Parent = workspace
	```
  6. Double-click `LevelNameHere` in `Workspace` and rename it to whatever you want your level to be named. This is your level folder.
     
* Get it from the Creator Marketplace:
  1. Go [here]() <!--TODO: Add link--> and click Get Model, then Try in Studio. 
  2. Open the Toolbox (View tab > Toolbox) and click the tab with an icon of 4 boxes.
  3. Find `Block Labs Kit` and click it to insert it. It should be the first result.
  4. With the kit selected, run this code in the command bar (View > Command Bar, look at the bottom of the screen):  
	```lua
	local kit = game.Selection:Get()[1]
	kit.Blocks.Parent = game.ReplicatedStorage
	kit.LevelNameHere.Parent = workspace
	```
	5. Double-click `LevelNameHere` in `Workspace` and rename it to whatever you want your level to be named. This is your level folder.
 
* Use the plugin:
  1. Open the Plugins tab in Studio.
  2. Find the `Block Labs Editor Plugin` and click `Insert`, then `Full Kit`.
 
## 1b. Getting the plugin (Optional, 2 min.)
Even though the plugin is optional, it takes less than 5 minutes to get and provides some helpful features:
* Add the kit in just two clicks
* Add objects without inserting the kit
* See this documentation without opening your browser
* Easily [create custom blocks](/tutorials/custom-blocks.md)
* Automatically move objects into your level folder

Download the plugin for free [here]()! <!--TODO: More steps, add link-->

# 2. Adding objects (2 min.)
To add an object, select it and duplicate it by pressing `Ctrl+D` (or `Cmd+D` for Mac). Then, use the Explorer to drag the object into your level folder.

>[!TIP]
>If you have the plugin, duplicated objects will automatically be put in your level folder.

Some objects, such as [buttons](/objects/buttons), have properties you can change. For example, [door buttons](/objects/buttons/door) have a [DoorToOpen](/objects/buttons/door#DoorToOpen) property. To change these properties, expand the object by clicking the arrow next to the name and picking a property. Then, change the `Value` in the Properties window (View > Properties).

If you're confused about what all the properties do, select a property and click the `What's this?` button on the plugin menu. If you don't have the plugin, you can also look for the property on its object's page in the Properties section.

# 3. Applying your knowledge (5 min.)
Now that you know how to add and edit objects, let's put this to use! Open Studio, press `Ctrl+N`/`Cmd+N` to create a new file, and add the kit. Next, you get to use your creativity! Lay out a map with basic Roblox parts. Change color, material, etc. using the Model tab or Properties window to make it look great! Don't forget to anchor everything and put it all in the level folder.

>[!IMPORTANT]
>Add parts by going to the Model tab and clicking the Part button. You can click the dropdown arrow underneath it to pick from other types, like cylinders, spheres, and wedges!

Once you have a good map, start adding objects to make your level... an actual level! You can do whatever you want, but for this tutorial, go ahead and add a button. Duplicate and drag. Put this button anywhere you want! Now add a door. Duplicate and drag. Put this somewhere else. Finally, add a spawner. You guessed it - duplicate and drag! If you'd like, you can also add a [light](/objects/light) to get rid of those pesky shadows.

Here's an example of what your level might look like:

<img width="450" alt="Example screenshot" src="https://github.com/user-attachments/assets/4b36ef7b-ba11-45cf-b300-9a57fd681569" />\
<sup>Example screenshot</sup>

>[!TIP]
>You might start to notice how annoying it is to move the parts into the level folder. If you don't want to get the plugin for some reason, run this command in the command bar after you duplicate an object:
>```lua
>for _, v in pairs(workspace:GetChildren()) do
>    if v:HasTag("LevelFolder") then
>        game.Selection:Get()[1].Parent = v
>    end
>end
>```

Hopefully that wasn't too hard! Next, we need to change the properties. First, let's connect the button and the door together. Expand the button in the Explorer to reveal the properties. Click on DoorToOpen, then on the Value field in the Properties window. Your cursor should change! Now, click on the door **in the Explorer.** If you click the door in the viewport, which is the screen in the middle, you might get an error once you test your work!

What you just changed is called an Instance value! When you try to change Instance values, you have to select something from the Explorer instead of typing.

>[!NOTE]
>An Instance, in Roblox terms, is something you add to your game to make it function. This includes parts, folders, scripts, and even GUI! You can use any Instance in your level except scripts, because those are disallowed.

It's time to playtest, but first, move the spawn into the level. Now we can go! Press `F5`. Try spawning a block and pushing it into the button! If you set up the properties correctly, the door will open. But... nothing's behind the door. That's kinda boring.

Build another room behind the door so you can add an exit. Adding the exit is nice and easy: just duplicate the [exit object](/objects/exit) from the kit, and... *drumroll please...* **DRAG!** Whoa, what a plot twist! 

You might notice that the exit part does absolutely nothing. This is intended. The ✨ *magical developer people* ✨ will make it work with their ✨ *magical developer spells* ✨ so that you don't have to lift a finger!

Ok! Now you're done! Good job. Playtest your work and see how epic it is!

See you next time! :)

---

<sup>PS: You probably noticed that the ending of this article was a bit more fun and the start was... nerdy and boring. The mood of this article is pretty much just whatever my mood was when I wrote it, so it's pretty inconsistent. Sorry about that! Anyway, you are now manually breathing. Goodbye!</sup>

<sup>© Orbit Productions 2025</sup>
