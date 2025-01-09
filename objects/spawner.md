# Block Spawner
A **Block Spawner**, usually shortened to **spawner**, is an object used to spawn [blocks](/objects/block). This is pretty essential to any level, so you should always include at least one spawner in anything you make.

# Usage
When its button is pressed, it will spawn the block specified in the `BlockToSpawn` property on top of the "Block Spawn" text. It'll also delete any blocks created by spawners with the same `SpawnerID`, including itself.

# Properties
|Property    |Acceptable Values                      |
|------------|---------------------------------------|
|BlockToSpawn|The name of any [block](/objects/block)|
|SpawnerID   |Any text (typically a number)          |

# Tips
* Change the `SpawnerID` property to create multiple blocks at the same time!
* You can delete the gray part to make a custom spawner.

---

<sup>© Orbit Productions 2025</sup>
