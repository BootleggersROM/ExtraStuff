# Build Variables for Bootleggers

This guide will include additional variables that you can use at the time of building the ROM. For a basic building guide, please refer to [our manifest](https://github.com/Bootleggers-BrokenLab/manifest/README.md). 

## Exportable variables

*NOTE: You can add any of the variables on your `bootleg_device.mk` (just adding a line of code like `EXPORTABLE_VARIABLE:=value`) or export on your shell by using the `export EXPORTABLE_VARIABLE=value` command for testing purposes.*



**BOOTLEGGERS_IS_LARGE_DEVICE** *(default value: true)*

Allows you to set if your device has a larger (generally in a 18:9) screen resolution. This is being used for wallpapers (default and system wallpapers).

This was added because we design our wallpapers in portrait, and for better compatibility (or in case we need a centered logo in the wallpaper), we add this to adapt our wallpapers in the best way possible.



**WITH_GAPPS** *(default value: false)*

Allows you to ship your build with gapps included. 

For some people gapps are an essential thing and for some other people is a huge privacy concern to have them, so we allow the choice of allowing both ways of building the ROM. We prefer not to have gapps in mind because it's the best of both worlds.



**WITH_MICROG** *(default value: false)*

Allows you to ship your build with MicroG support. 

TODO: Add a repo with a bundle of FOSS apps.



**BOOTLEGGERS_BUILD_APPS_BUNDLE** *(default value: true)*

Allows you to ship a bundle of apps. These apps are a calculator, a calendar, a notes app, a gallery app and a music player.

We include this apps because these are mostly needed when you go out or in any circunstance. But if you prefer a cleaner system, you can disable them. This applies also to gapps. 

Our list of bundled apps (currently, this might be changed) is the following:


| **App category** | **Non-gapps variant**      | **Gapps variant** |
|------------------|----------------------------|-------------------|
| Browser          | Jelly                      | Google Chrome     |
| Calendar         | Etar                       | Google Calendar   |
| Calculator       | AOSP Calculator            | Google Calculator |
| Gallery          | Quickpic (WSTProjects Mod) | Google Photos     |
| Notes app        | Notally                    | Google Keep       |
| Music Player     | Auxio                      | YouTube Music     |