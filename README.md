# How to Maximize Your FPS in VRChat

This is a guide that explains what software settings you can change - both in and out of VRChat - in order to get the most performance or FPS possible. Please note that performance gains are made by sacrificing some quality, so I encourage you to try changing settings and find a balance that you're happy with. While this guide has a PCVR focus, you should be able to apply the non-VR changes and increase your FPS in desktop mode (or on Android/standalone Quest) as well.

If you are looking for computer hardware recommendations, I recommend checking out [Tupper's guide](https://tupper.notion.site/The-Current-Best-PC-For-VRChat-0636cbf57062499e80f02554afda2be4). It's very good, and explains what hardware specs you want to focus on to maximize performance. For hardware recommendations on a budget, I recommend asking [/r/buildmeapc](https://reddit.com/r/buildmeapc/).

## Summary
**This is a detailed guide, so here is a brief summary of the changes you can make that have the biggest impact on FPS:**
- Set your headset refresh rate to 90hz
- Set your headset resolution to 80%
- Turn on avatar culling (e.g. 20m and max 15)
- Set Anti-Aliasing to x2
- Turn off avatar shaders
- Turn off nameplates in crowded instances

If you want more details or information on where these settings are located, please keep reading! Key parts are bolded.

## In-Game Graphics and Avatar Settings

![](images/settings_graphics_1.png)

![](images/settings_graphics_2.png)

![](images/settings_avatars_1.png)

### Block Poorly Optimized Avatars
While you can block very poor or poor avatars with this setting, **I recommend turning off avatar shaders instead (see [Safety Settings](#in-game-safety-settings))**. This allows you to see a general idea of what an avatar looks like, rather than seeing the "Perf Blocked" robot avatar.

### Max Avatar Download Size
**This won't have a direct effect on your FPS**, but larger avatars tend to be worse quality, so limiting size can indirectly increase your FPS. Rather than changing this, I again recommend turning off avatar shaders instead.

### Dynamic Bones
**Make sure "Convert Dynamic Bones To PhysBones" is On.** This will automatically convert Dynamic Bones on old avatars to PhysBones, which is VRChat's optimized implementation.

### Graphics Settings
Max Performance:
- **Anti-Aliasing: x2**
- Mirror Resolution: Quarter
- Shadow Quality: Low
- LOD Quality: Low
- Particle Physics Quality: Low
- Particle Limiter: On
- Pixel Light Count: Low

**Turning Anti-Aliasing off can have a large negative impact on quality, as well as break some worlds/shaders, so I recommend an x2 minimum.** Addtionaly, it's possible to change Pixel Light Count to Off, but this can also have a large negative impact on quality, so I recommend Low.

### Avatar Culling Settings

**By lowering the avatar culling distance or number of avatars you show, you'll increase your FPS**, but you'll see more diamond avatar replacements.

### Additional Settings

**Turning off nameplates in crowded instances can increase your FPS.** The quickest way to access this setting is the mini menu Settings tab.

## In-Game Safety Settings

![](images/settings_safety_1.png)

These are the safety settings that I use for all trust levels. A decent amount of GPU processing is spent on shaders, so **I recommend turning off shaders for non-friends of all trust levels**. If you have a large number of friends in an instance, you can also turn off friends' shaders to gain FPS. This will make some avatars look weird (like making them entirely one color), but you'll be able to generally see what avatars look like, and you can then decide if you want to show their avatar or not. Manually showing someone's avatar overrides this setting, regardless of trust level.

## Steam Launch Options

![](images/launch_options_1.png)

![](images/launch_options_2.png)

While in VR, VRChat also runs in a desktop window on your computer. Making this window smaller can increase headset FPS. To do this, open VRChat's properties on Steam by right-clicking on the game in your library, and add the following to the Launch Options:

```-screen-width 640 -screen-height 480```

Please note that the in-game Stream Camera uses the desktop window for output. If you are streaming/recording, you will want to leave this alone, or maximize the window before streaming/recording.

## Headset Settings

Every headset *should* have a settings menu where you can adjust refresh rate and render resolution. For SteamVR headsets, make sure your headset is plugged in and turned on, then click the hamburger menu in the top left corner of the SteamVR window.

![](images/steamvr_1.png)

![](images/steamvr_2.png)

**The lower the render resolution, the higher your FPS.** In my experience, you can lower this to 80-90% and not be able to tell the difference in quality at all, while increasing your FPS.

**Lowering your refresh rate can also increase your performance**, but the lower refresh rate can be very noticeable. I don't recommend going lower than 90hz.

## Quest Link Apps

If you have a Quest headset that you connect to your computer in order to play PCVR games, there are several apps available to you. People report different levels of performance with all of these, so I recommend trying them out and seeing which works best for you. Please note that these apps can require additional setup/hardware and are recommended for advanced users.

- [Virtual Desktop](https://www.meta.com/experiences/2017050365004772/) ($19.99): Widely considered to provide the best performance, but not free.
- [Steam Link](https://www.meta.com/experiences/5841245619310585/) (Free): Valve's official link app.
- [ALVR](https://github.com/alvr-org/ALVR) (Free, FOSS): Free and open source alternative.

## Other Tips

These aren't directly related to VRChat/VR, but they can increase your performance as well:
- Apply any Windows updates and restart your computer before launching VRChat
- Make sure your graphics drivers are up to date
- Close un-needed apps (and make sure they're actually closed, not just minimized in the taskbar)

## Conclusion

Thanks for reading! I hope my guide was able to help you increase your FPS in VRChat. If you have any comments/questions/etc, please feel free to [open an issue](https://github.com/shugy0/max-vrchat-fps/issues).

The world in the background of the screenshots is [Moment by Alia-](https://vrchat.com/home/world/wrld_f3e56230-2bd9-4688-86eb-e24fa3e4c595).

DISCLAIMER: This guide is an independent publication and has not been authorized, sponsored, or otherwise approved by any of the companies or entities mentioned within. References to any specific game, software, hardware, or company are for informational purposes only and do not imply endorsement or affiliation. The information outlined in this guide is based on personal experience and research and should be applied at your own discretion. The authors and publisher of this guide are not responsible for any outcomes that may arise from the application of the information provided.

LICENSE: https://creativecommons.org/licenses/by/4.0/