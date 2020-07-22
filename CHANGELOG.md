![Banner](graphics/banner.jpg)

This file documents all notable changes to ksp-albedo.

This CHANGELOG is in compliance with [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Psyrr-Era Current Development

### V 0.2.6

* Added CHANGELOG to keep track of notable changes to project.
* New In-Depth README.md
* 

## Valarian-Era Prior Development

### V 0.2.5.2 - 2016-10-04
- Recompiled to fix issue with KSP build 1564
 
### V 0.2.5.1 - 2016-09-14
- Updated for KSP 1.2 pre-release
- Does not work with KSP 1.1.* or older
 
### V 0.2.5 - 2016-04-04
- Updated for KSP 1.1
- Does not work with KSP 1.0.* or older
 
### V 0.2.4.2 - 2015-11-28
- Fixed missing shadows when orbiting close to the sun
- Fixed vessel suddenly turning pitch black when deep underwater
 
### V 0.2.4.1 - 2015-11-25
- Removed the obsolete Real Solar System colors and useless README.txt
 
### V 0.2.4 - 2015-11-25
- Fixed a bug that prevented the stock toolbar icon settings to be saved correctly.
- Fixed a bug that sometimes displayed unintended atmospheric lights on all other bodies when in map/orbit view.
- A bit of code cleaning and refactoring, might even improve performance and stability.
 
### V 0.2.3.1 - 2015-05-10
- Fixed the bug that created multiple toolbar buttons (sorry for that)
- The config node name for celestial bodies has been renamed from "CelestialBodyColor" to "PlanetshineCelestialBody", however retro-compatibility will be kept for some time
- The celestial bodies are now loaded through "GameDatabase", meaning that:
    * any "PlanetshineCelestialBody" node within any cfg file in the GameData folder will be loaded automatically
    * other plugins can programatically change "PlanetshineCelestialBody" nodes through "GameDatabase"
    * "PlanetshineCelestialBody" nodes are now affected by Module Manager
 
### V 0.2.3 - 2015-05-09
- Fixed the bug preventing to save settings
- Added support for stock toolbar (blizzy's toolbar is no longer required, but still supported)
- Added a "close" button to the settings window
- Tweaked the default settings, now it's a tiny bit brighter in space

### V 0.2.2.3 - 2015-05-03
- Updated the version file for KSP 1.0.2

### V 0.2.2.2 - 2015-04-30
- Updated the version file for KSP 1.0

### V 0.2.2.1 - 2014-12-20
- Updated the version file for KSP 0.90
 
### V 0.2.2 - 2014-10-20
- Included a custom planets/moons color file to use with the mod Real Solar System
- Vacuum ambient light level can now be set MUCH brighter
- New option in "CelestialBodies.cfg" to change the level of ground ambient overriding (I made it mostly for compatibility with RSS)
- Fixed some small typos and tweaked some calculations a bit
 
### V 0.2.1 - 2014-10-18
- Fixed a bug that occurred when starting in single light mode
- Added a performance option to change the update frequency
- Added a "reset to default" button for each setting
- Fixed the ground albedo formula for when there is no atmosphere

 
### V 0.2.0 - 2014-10-17
- Comprehensive settings menu (requires Toolbar)
- Settings have moved and are no more meant to be edited outside of the game
- Added quality preset options (low, medium, high)
- New ground ambient light enhancement system
- Fixed several light angle calculation bugs
- Added option to choose between vertex or pixel lights
 
### V 0.1.4 - 2014-10-15
- Added support for Add-on Version Checker and included "MiniAVC"
- Added minimal debug menu to toggle the effects (requires Toolbar)
- Performance improvement: forced vertex lights

### V 0.1.3 - 2014-10-14
- Renamed the mod from "Reflective Ambient Light" to "Planetshine"
- Fixed a bug that caused an error on loading
- Improved performance

### V 0.1.2 - 2014-10-13
- Improved performance

### V 0.1.1 - 2014-10-12
- Much more options and explanations within the config files, I strongly suggest to look into them
- Fixed a bug that made the light suddenly disappear when at sunset/sunrise, instead of doing it smoothly
- Fixed a bug that made the light always come from the center of the planet instead of the actual illuminated part of the surface
- The sun now has its own light setting, orbiting close to it has a VERY STRONG effect 
- Added the option to change the ground atmosphere ambient intensity (the ambient light when you are on the ground) in the settings
- Added the option to change the atmosphere ambient altitude fading
- Added the option to change the light reflection effect atmosphere altitude and fading
- Added the option to change the maximum orbital range of the light reflection
- Added the option to set the ratio of atmosphere ambient on ground for each planet/moon
- Added the option to disable the area light technique in order to get better performance (by default it uses 3 lights to simulate an area, but if you disable it it will only use one light)
- On planets/moons without atmosphere, the reflective light is more spread around the ship when landed
- Tweaked many settings to improve the light effects

### V 0.1.0 - 2014-10-11
- First released version
- Each planet/moon has a different color, picked from a config file
- Effect range is 4x the radius of a planet/moon
- The effect strength can be changed in the settings file
