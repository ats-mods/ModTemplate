# Against The Storm Mod Template

This is a basic template for an Against the Storm mod. Because ATS is a unity game, existing mod loaders and techniques can be leveraged to easily create a mod.

The compiled mod is meant to be loaded into the game with [BepInEx](https://github.com/BepInEx/BepInEx). I tested with the x86 version [5.4.2](https://github.com/BepInEx/BepInEx/releases/download/v5.4.21/BepInEx_x86_5.4.21.0.zip). Simply download the loader and unzip it into your game directory. For the Steam version of the game, this will likely be `C:\Program Files (x86)\Steam\steamapps\common\Against the Storm\`. 

The `.dll` file created by this mod (`ModTemplate.dll` by default) can then be dropped into the `BepInEx\plugins` subdirectory inside the game directory. You might have to make this directory yourself, or run the game once to have it made automatically.

This plugin template was initiated from BepInEx plugin template command:

```bash
dotnet new bepinex5plugin -n ModTemplate -T netstandard2.0 -U 2021.3.15
```