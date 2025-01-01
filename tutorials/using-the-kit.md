This tutorial explains how to use the kit and the optional plugin. Watch the video on [the Tutorials page](/tutorials) to learn how to use Roblox Studio.

Skill level: **Beginner**\
Length: **~5 min.**

# 1. Getting the Kit (2 min.)
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
  6. Rename `LevelNameHere` in `Workspace` to whatever you want your level to be named. This is your level folder.
     
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
	5. Rename `LevelNameHere` in `Workspace` to whatever you want your level to be named. This is your level folder.
 
* Use the plugin:
  1. Open the Plugins tab in Studio.
  2. Find the `Block Labs Editor Plugin` and click `Insert Kit`.
 
## 1b. Getting the Plugin (Optional, 2 min.)
Even though the plugin is optional, it takes less than 5 minutes to get and provides some helpful features:
* Add the kit in just one click
* Add objects without inserting the kit
* Open templates from inside Studio
* See this documentation without opening your browser
* Easily [create custom blocks](/tutorials/custom-blocks.md)

Download the plugin for free [here]()! <!--TODO: More steps, add link-->

# 2. Adding objects (2 min.)
To add an object, select it in the Explorer (View > Explorer) and duplicate it by pressing `Ctrl+D` (or `Cmd+D` for Mac). Then, drag the object into your level folder.

Some objects, such as [buttons](/objects/buttons), have properties you can change. For example, [door buttons](/objects/buttons/door) have a [DoorToOpen](/objects/buttons/door#DoorToOpen) value. To change these properties, expand the object by selecting it, clicking the arrow next to the name, and picking a property. Then change the `Value` in the Properties window (View > Properties).
