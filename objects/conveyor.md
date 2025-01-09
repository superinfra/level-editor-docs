# Conveyor
A **conveyor** is an object that pushes any blocks or players on its surface in the specified `Direction`.

# Usage
Set the `Direction` and anything that touches its surface will be moved in that direction! You can change also change the `Speed`. If you place a block on the first end of a conveyor and buttons on the other end, you can make a Conveyor Script! These are useful for binding multiple actions to one trigger.[^1]

# Properties
|Property |Acceptable Values|
|---------|-----------------|
|Direction|Any Vector3      |
|Speed    |Any number       |

>[!IMPORTANT]
>A Vector3 is a set of 3 comma-separated numbers representing direction, position, and anything related to 3D space. The first number is the X-axis (length), the second is the Y-axis (height), and finally, the Z-axis (depth).[^2]
>
>For example, if you input `1, 0, 0` and stand on the conveyor, you will be moved horizontally across the conveyor on the X-axis. If you input `1, 0, 1`, however, you'll be moved diagonally since the conveyor is now moving you on the X-axis <ins>*and*</ins> the Z-axis.

[^1]: Learn more at the [Conveyor Scripting tutorial](/tutorials/conveyor-scripting.md).
[^2]: See the official Roblox documentation here: <https://create.roblox.com/docs/en-us/reference/engine/datatypes/Vector3>

---

<sup>© Orbit Productions 2025</sup>
