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
To add an object, select it and duplicate it by pressing `Ctrl+D` (or `Cmd+D` for Mac). Then, drag the object into your level folder using the Explorer.

>[!TIP]
>If you have the plugin, duplicated objects will automatically be put in your level folder.

Some objects, such as [buttons](/objects/buttons), have properties you can change. For example, [door buttons](/objects/buttons/door) have a [DoorToOpen](/objects/buttons/door#DoorToOpen) property. To change these properties, expand the object by clicking the arrow next to the name and picking a property. Then, change the `Value` in the Properties window (View > Properties).

If you're confused about what all the properties do, select a property and click the `What's this?` button on the plugin menu. If you don't have the plugin, you can also look for the property on its object's page in the Properties section.

# 3. Applying your knowledge (5 min.)
Now that you know how to add and edit objects, let's put this to use! Open Studio, press `Ctrl+N`/`Cmd+N` to create a new file, and add the kit. Next, you get to use your creativity! Lay out a map with basic Roblox parts. Change color, material, etc. using the Model tab or Properties window to make it look great! Don't forget to anchor everything and put it all in the level folder.

>[!IMPORTANT]
>Add parts by going to the Model tab and clicking the Part button. You can click the dropdown arrow underneath it to pick from other types, like cylinders, spheres, and wedges!

Once you have a good map, start adding objects to make your level... an actual level! You can do whatever you want, but for this tutorial, go ahead and add a button. Duplicate and drag. Put this button anywhere you want! Now add a door. Duplicate and drag. Put this somewhere else. Finally, add a spawner. You guessed it - duplicate and drag!

>[!TIP]
>You might start to notice how annoying it is to move the parts into the level folder. If you don't want to get the plugin for some reason, run this command in the command bar after you duplicate an object:
>```lua
>for _, v in pairs(workspace:GetChildren()) do
>    if v:HasTag("LevelFolder") then
>        game.Selection:Get()[1].Parent = v
>    end
>end
>```

Hopefully that wasn't too hard! Next, we need to change the properties. Change all the properties in this table to the right values:

|Object|Property  |Value|
|------|----------|-----|
