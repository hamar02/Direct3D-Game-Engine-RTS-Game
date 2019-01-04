Build D3DDemo.sln, Win32

Techniques:
Normal Maps.
Blend Mapping in Terrain Shader & Moving Lava.
Physically Based Rendering.
Shadow Map, uses same rotation as the camera, from directional light.
Frustum Culling.
Terrain Generator from height map.
Entity & Component System.
A* pathfinding, creates nodes from the terrains vertices and a "pathable/unpathable" texture.
Unit & Unit Orders.
Some very basic behavior tree in the bot.



GAME

Controls:
WASD and cursor at the corner of the screen will move the camera.
Left click to select unit.
Left drag click to select multiple units.
Right click with a unit selected to give an order to the units.

About the game:
The player (blue), fights against the bot (red).
It's a battle royal RTS, so the last standing main tank wins.
Main tanks can gather gold directly from the gold mine and capture buildings.
Refinery building can produce workers at the cost of 120 gold.
Workers can gather gold from the gold mine, but has to return it to a refinery compared to the main tanks. 
Baracks can produce fighters at the cost of 160 gold.
Fighters can attack enemy units.

The lava will move one step closer to the center of the map at 9.40.
Another step around 8 and then it will move to it's final step at 6.

Known bugs:
Workers stop working if they lose "their" refinery.
Drag select multiple units, only works in down right corner of map.
Camera can't move left. It can, just keep hitting the A button. Somehow it gets stuck when moved to the far right of the map.
Memory leak.. We think we're mistreating ImGUI.