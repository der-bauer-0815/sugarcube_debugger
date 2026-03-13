# sugarcube_debugger
This is a lightweight, single-file HTML tool designed for debugging and cheating in local browser games built with the Twine/SugarCube engine.
# SugarCube Local Debug Tool

This is a lightweight, single-file HTML tool designed for debugging and cheating in local browser games built with the Twine/SugarCube engine. 

Whether you are a developer/player looking to test specific game states, or a player wanting to tweak your stats and inventory, this tool allows you to inspect, modify, and freeze the game's internal variables in real-time.

## ✨ Features
* **Live Variable Inspection:** View a real-time, collapsible tree of all active game variables (`SugarCube.State.active.variables`).
* **On-the-Fly Editing:** Directly change the values of strings, numbers, and booleans while playing.
* **Value Freezing:** Lock a variable to a specific value. Even if the game's code tries to change it, the tool will instantly force it back to your desired value (perfect for locking health, money, or stats).
* **Quick Filtering:** Use the search bar to instantly find the exact variable you are looking for among hundreds.
* **Side-by-Side UI:** Plays the game in a large left panel (80% width) while keeping your debug controls accessible in a right panel (20% width).

---

## ⚠️ CRITICAL: Folder Placement for Assets
For the game to look and function as intended, **you must place this tool's HTML file in the exact same folder as the game's HTML file.**

If you run this tool from a different location, the relative file paths will break, and the game will not be able to load any of its local assets (images, videos, GIFs, audio files, etc.). 

---

## 🛡️ 100% Local & Private
This tool is completely self-contained within a single HTML file. **It is strictly a local tool and performs absolutely no communication with external servers or the internet.** No scripts, CSS, or data are downloaded from or uploaded to the web. Your game state and files never leave your machine.

---

## 🚀 How to Use

1. **Download** the `debugger.html` file from this repository.
2. **Move** the `debugger.html` file into the exact same folder where your target SugarCube game's `.html` file is located.
3. **Open** `debugger.html` in your web browser of choice.
4. **Import** the game by clicking the file input button on the launch screen and selecting the game's `.html` file from that same folder.
5. **Play & Modify:** The game will load on the left. Use the right panel to search for variables, change their values, or toggle the "Freeze" button to lock them in place.

## Compatibility
This tool is designed specifically for HTML files compiled using the Twine/SugarCube format. It hooks directly into the `SugarCube.State` API. It will not work with other Twine story formats (like Harlowe or Snowman) or games built on different engines.