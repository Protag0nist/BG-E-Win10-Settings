# Beyond Good & Evil - Fixing Several Windows 10 Bugs & Problems 
These are the settings that I use to let me run the game with a minimal amount of issues. With these settings I no longer experience audio de-sync issues, animations that play to quickly, graphical glitches, etc. The game runs near perfect for me with these options. The main (& currently only issue) I'm having at the moment is that occasionally some text on MDiscs bugs out. I suspect this issue occurs due to the resolution I play at but will need to perform further tweaks & testings on this.

I've saved these settings on Github so there archived &amp; to potentially help others that have ran into similar problems.

## Nvidia Control Panel Settings
Manage 3D Settings -> Program Settings
    ```Select bge.exe from the drop down, or find it in your Steam install location (<YOUR STEAM DIRECTORY>\steamapps\common\Beyond Good and Evil\BGE.exe)```
- FXAA = On
- Low Latency Mode = Ultra
- Monitor Technology = Fixed Refresh
- Preferred Refresh Rate (your monitor model) = Application Controlled
- Vertical Sync = On (Try with this setting off first. I needed to have it on due to severe screen tearing.)
By forcing a specific refresh rate for the game, it resolved a lot of my problems. This is because my monitor's refresh rate exceeded what the game was built for.

## Options within the Settings Application
```Default directory is \<STEAM DIRECTORY LOCATION>\steamapps\common\Beyond Good and Evil\SettingsApplication.exe```


Advance Settings  || All on or max
Advance Settings  || Manual Compatability Settings = On
Advance Settings  || Manual Compatability Settings = All on
Graphics Settings || Video card = Whatever your monitor is attached to
Graphics Settings || Resolution = Your preferred
Graphics Settings || Refresh Rate = 60Hz
    
## Fixing Audio De-Sync & 'Speedy' Animations
The best (& least sketchy) way of tackling these issues is by capping your game's frame rate, that way you're not downloading suspicious DLL files & other things. I use Rivatuner Statistics Server to do this & I set the cap to 30 fps. You can try experimenting with higher frame rates but I wouldn't recommend anything about 60 fps because you'll start to run into problems. At 30 the game is still very much playable.

### Eww, why do I need to cap my game to a low frame rate?
BG&E originally came out in 2003, it's an old game. As stated above, the game was built for devices that ran at low frame rates & low refresh rates when compared to today's devices. So, when today's computers complete the calculations for old games they do so too quickly & it causes problems. For those that own Hitman: Blood Money on PC & have played above 60 FPS you will have experienced this effect happening on the slops of 'A Vintage Year' - [See example here](https://www.youtube.com/watch?v=Lc1H3uYIbjk). The player can't run down the path, they get stuck because of this reason. 60 FPS or lower & 47 will run down as designed. 

TLDR; A common solution to a lot of 'legacy titles / retro gaming' problems is to run the game at a capped frame rate. 
