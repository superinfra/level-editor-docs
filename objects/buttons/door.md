# Door Button
A **door button** is a type of **button** used to open [doors](/objects/door.md). This is the most basic puzzle element, but it can also be used to start a [conveyor script](/tutorials/conveyor-scripting.md)!

# Usage
When pressed by a block, it will open the door specified in the `DoorToOpen` property. If `PlayerActivated` is true, then this behavior is triggered by a player instead of a block.

# Properties
|Property       |Acceptable Values|
|---------------|-----------------|
|DoorToOpen     |Any door         |
|PlayerActivated|True or false    |

>[!CAUTION]
>If you change the `DoorToOpen` property using the viewport (the preview in the middle of the screen), it may error. You should always click on the door you want using the Explorer.

---

<sup>© Orbit Productions 2025</sup>
