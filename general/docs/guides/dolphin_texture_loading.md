# Dolphin Texture Loading

The Dolphin Emulator has a built-in way to load your own textures into the game. As of version 5.0 you will find these two options under the Advanced tab of Graphics Configuration:

![Dolphin Load/Dump Textures](/general/images/tools/dolphin_load_dump_textures.png?raw=true "Dolphin Load/Dump Textures")

## How to Dump Textures

To dump textures, make sure that the option in the above image for Dump Textures has been selected. Then you will want to launch the game and encounter the texture. When the game attempts to load the texture, it will dump it to your Dolphin documents folder. On Windows this folder defaults to `C:\Users\<your user>\Documents\Dolphin Emulator\Dump\Textures`.

In the textures folder you will find a folder created (named G4NJDA for Naruto GNT4 or SNXJDA for Naruto GNT SP), which is the folder that contains the dumped textures for the game.

## How to Load Textures

To load textures, make sure that the option in the above image for Load Custom Textures has been selected. For your specified game, modify the textures you found in `Dump\Textures\<game_id>` and copy them to `Load\Textures\<game_id>`. Make sure that you do not modify the name or dimensions of the image. You can logically separate the images by creating subfolders in `Load\Textures\<game_id>`, as Dolphin will recursively search for textures in this folder. When you start the game, any textures in this folder will be loaded. If a custom texture is loaded, it will not be dumped to the `Dump\Textures\<game_id>` folder. You can also turn Load Custom Textures on and off without having to restart the game.

## Resource Packs

A new update was introduced with Dolphin 5.0-9217, [Implement Resource Packs](https://dolphin-emu.org/blog/2019/02/01/dolphin-progress-report-dec-2018-and-jan-2019/#50-9217-implement-resource-packs-by-spycrab). Any texture packs that say they use the new resource pack format can be added using this new **Resource Pack Manager** menu.