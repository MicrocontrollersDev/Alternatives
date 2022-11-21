# Migrating to Latest (1.19.2)

This is a comprehensive guide on how to download Fabric and mods for it. It also provides direct links to many mods that you may find useful.

## Introduction

If you want more information on Fabric, why Forge/OptiFine are not recommended, or need help downloading Fabric and mods for it, click on the `Introduction` drop down below. If you are just here to see the mods list, continue to the next section.

??? note "Introduction"

    ### The Situation

    So, you've been playing 1.8 for the past [6.5 years](https://howoldisminecraft189.today) and are ready to see what 1.19 has to offer. Your first thought may be to download and install Forge and then add OptiFine as a mod, but this could not be further from the best choice. As Mojang has been rolling out releases, they've also been decreasing performance with every version, and neither Forge nor OptiFine are really able to bring back even a speck of that performance we see in 1.12 and below. However, another mod loader, Fabric, which is lightweight and easier to develop for, has created an amazing community in which many of its members focus on helping optimize the game to its greatest potential.

    ### Why no longer OptiFine?

    OptiFine no longer provides the benefit that it once did on older versions of the game. As the years have gone by and Minecraft's code has changed, OptiFine has been continuing to completely overwrite major parts of Minecraft's code. Because OptiFine is closed source, it has become increasingly harder for modders to provide OptiFine compatibility. OptiFine also uses outdated formats for many of its features, including MCPatcher and its confusing and outdated settings menu. Many members in the Fabric community have taken it upon themselves to create better performance enhancing mods which surpass OptiFine, as well as provide alternatives to many of OptiFine's iconic features.

    While there is a Fabric compatibility layer for OptiFine known as OptiFabric, it is unsupported by many of the mods on the list, with some outright preventing the game from loading if OptiFabric is present. Therefore, consider all mods in this list to be incompatible with OptiFabric.

    ### Why no longer Forge?

    Forge has always been less than ideal for performance due to its large overhead for server-sided modding, which is not necessary for users wishing for a vanilla compatible experience. Fabric on the other hand is extremely lightweight and is practically identical to vanilla. It's also considered to be much easier to make mods for and is being used as the stepping stone for [Quilt](https://quiltmc.org/faq), an in-progress mod loader which will provide many more benefits to modders and users alike.

    ### Installing Fabric

    This is only for the default Minecraft launcher. If you are using [Prism Launcher](https://prismlauncher.org), you can easily create a new profile and install fabric to it. It is highly recommended to use Prism Launcher instead of the default launcher as it provides many more features for both modders and regular users alike.

    0. Make sure you close Minecraft and the Minecraft launcher before installing Fabric, otherwise unexpected things can happen.
    1. Download the [Fabric installer](https://fabricmc.net/use).
        - If you are on Windows, use either the `.JAR` version on the left or the `.EXE` version of the installer on the right.
        - If you are on any other operating system or the `.EXE` version is not working for you, then use the `.JAR` version on the left.
    2. Run the installer.
        - If you are using the `.EXE` version of the installer, simply double click the file. You may get a popup blocking you from running the installer and saying that "Windows protected your PC"; if so, click on `More info` and then `Run anyway`.
        - If you are using the `.JAR` version, you will need to have Java installed on your device. If you have Java installed, double click the downloaded file to run the installer. If you don't, then follow these steps:
            1. Go to the [Java downloads page](https://adoptium.net/?variant=openjdk17&jvmVariant=hotspot) and download the version of Java corresponding to your device.
            2. Run the Java installer by double clicking it.
            3. Do whatever the installer tells you to do.
            4. After installing Java, you should be able to run the Fabric installer by double clicking it. If you still can't for some reason, try running the program [Jarfix](https://johann.loefflmann.net/downloads/jarfix.exe).
    3. Now that you have opened the installer, you will see two tabs at the top of the window: `Client` and `Server`. Make sure you are on the `Client` tab. Then, open the `Minecraft Version:` dropdown and select the version of Minecraft you want (most likely the latest version of Minecraft). The rest of the settings can be left with their defaults (unless you store your Minecraft version files in a different folder - if you want to use a different directory for this installation, that should be changed in the Minecraft launcher, not here). Click on `Install` when you are ready to install Fabric.
    4. Once Fabric is finished installing, open your Minecraft launcher and click on the profiles button at the bottom left corner. Select the Fabric profile, it should be called something like `fabric-loader-1.19.x`. Then hit `PLAY` to start playing!
        - If you do not see the profile, try exiting and reopening the Minecraft launcher. If this also does not work, go to the `Installations` tab in the Minecraft launcher and make sure the `Modded` option is ticked on the rop right corner. If it still does not show up, create your own installation by clicking the `New installation` button, and selecting your desired fabric version in the `Version` dropdown. Then press `Create` and launch this installation.

    ### Downloading Mods for Fabric

    This list currently consists of three different sources for mod downloads: Modrinth, GitHub, and CurseForge. This section will explain how to download mods from each of them.

    - Modrinth:
        - On the mod's page, click on the `Versions` tab. From there, you can see all versions of the mod. Make sure you download the correct one based on the Minecraft version and mod loader, click on the download icon for the newest version of the mod that fits both previous criteria.

    - GitHub:
        - For your convenience, all GitHub links lead directly to the latest version of the mod. From here, click on the `Assets` drop down if needed, then download the jar that does not include `-sources` or `-dev` in the name.
            - If a link does not redirect you to the latest version but rather the main page, on the right side of the page, you should find a tag icon with the latest version. 

    - CurseForge:
        - Click on the `Files` tab. Look for the versions of the mod with the Minecraft version you desire and is for the Fabric mod loader, and download the latest one. You can also press the `View All` button, then sort by mod loader or Minecraft version to make finding the correct jar easier.

    If you are using Prism Launcher, you can simply go to the mods menu for your instance and press the "Download Mods" button in the top right to search Modrinth and CurseForge directly inside the launcher.

    **NOTE: SOME CURSEFORGE MODS MAY NOT ALLOW DOWNLOADS FROM THIRD PARTIES SUCH AS POLYMC**

    ### Installing Mods on Fabric

    This is only for the default .minecraft directory. If you have made a custom directory, you likely do not need this guide.

    0. Make sure you close Minecraft before installing mods, otherwise unexpected things can happen.
    1. Open your Minecraft folder:
        - Windows: Hold the Windows key (`win`) and press `r` to open the Run program. Then type in `%appdata%/.minecraft` and hit enter.
        - Mac: On the bar at the top of your screen in Finder, click `Go`, then click `Go to Folder` and type `~/Library/Application Support/Minecraft`, then hit enter.
        - Linux: Open `~/.minecraft`.
    2. In your Minecraft folder, open the folder called `mods`.
        - If this folder does not exist, create it.
    3. Place all of the mods you want to use into this folder (note that all mods you install must support Fabric 1.19 or they will not work).

    ### Still Need Help?

    Feel free to join my [Discord server](https://inv.wtf/micro) for any help downloading Fabric, its mods, or general questions about them.
    
## Mods

### NECESSARY

As of 1.19, Mojang has added the ability to report chat messages. While on the surface this sounds great, these chat reports do not go to the server owners, but to a Mojang moderation team. This team will then decide your punishment, which is a temporary or permanent ban from all online servers and Realms. **If you do not want to get banned from playing online, use this mod!**

| Mod | Description | Author |
| --- | --- | --- |
| [No Chat Reports](https://modrinth.com/mod/no-chat-reports) | Server side and client side mod. Prevents chat reporting from working if `enforce-secure-chat` is not enabled. Works best if installed on both sides but is not required. | [Aizistral](https://github.com/Aizistral-Studios) |

Are you a server owner using Bukkit, Spigot, Paper, or a similar plugin based server? Check out [Freedom Chat](https://modrinth.com/plugin/freedomchat) by [eim](https://github.com/e-im) for similar functionality to No Chat Reports!

### Dependencies

These are essential mods that are required for some fabric mods to work.

| Mod | Description | Author |
| --- | --- | --- |
| [Fabric API](https://modrinth.com/mod/fabric-api) | Required for most Fabric mods. | [Fabric Team](https://github.com/FabricMC) |
| [Fabric Language Kotlin](https://modrinth.com/mod/fabric-language-kotlin) | Required for mods that use Kotlin. | [Fabric Team](https://github.com/FabricMC) |
| [Mod Menu](https://modrinth.com/mod/modmenu) | Allows the user to see all installed mods in-game, as well as access the config for most. | [Terraformers](https://github.com/TerraformersMC) |
| [Architectury](https://modrinth.com/mod/architectury-api) | Required for a few mods. | [Shedaniel](https://github.com/shedaniel) |
| [Cloth Config](https://modrinth.com/mod/cloth-config) | Required for a few mods. | [Shedaniel](https://github.com/shedaniel) |
| [MaLiLib](https://www.curseforge.com/minecraft/mc-mods/malilib) | Required for a few mods such as Litematica. | [Matti Ruohonen](https://github.com/maruohon) |


### Performance

These are mods that are needed for playing the latest versions of Minecraft at a reasonable FPS. These will also help decrease frame times, hopefully eliminating spikes or stuttering.

| Mod | Description | Author | Incompatibilities |
| --- | --- | --- | --- |
| [Sodium](https://modrinth.com/mod/sodium) | An all around performance mod, Sodium allows users to play the latest versions of Minecraft with high FPS, completely outperforming OptiFine, with some users seeing up to 8x their vanilla frames. Sodium also drastically improve visuals, providing a much better gameplay experience. | [CaffeineMC](https://github.com/CaffeineMC) |
| [Iris](https://irisshaders.github.io) | A shader loader that allows users to load up their favorite OptiFine shaderpacks, but with much higher FPS. Iris also provides performance enhancements when not using shaders, making it great for all users. | [IrisShaders](https://github.com/IrisShaders) |
| [Indium](https://modrinth.com/mod/indium) | Adds FRAPI support to Sodium, making it necessary to use for some of the mods on this list to work. This mod is merely temporary and will be removed once Sodium adds FRAPI/FREX support itself. | [comp500](https://github.com/comp500) |
| [Lithium](https://modrinth.com/mod/lithium) | Helps improve the performance of many vanilla systems without changing their mechanics. | [CaffeineMC](https://github.com/CaffeineMC) |
| [Starlight](https://www.modrinth.com/mod/starlight) | Rewrites the light engine to make loading chunks much quicker. Please note that this does not maintain full vanilla parity (this will not effect most casual players). If you want complete vanilla parity or if Starlight is causing stutters, please look at [Phosphor](https://modrinth.com/mod/phosphor). | [SpottedLeaf](https://github.com/Spottedleaf) | Phosphor |
| [Exordium](https://modrinth.com/mod/exordium) | Caps the FPS of certain HUD elements that do not need to be updated every frame. | [tr7zw](https://github.com/tr7zw) | (May break some HUD elements. Currently, the crosshair has no transparency.) |
| [LazyDFU](https://modrinth.com/mod/lazydfu) | Prevents the DataFixerUpper from doing anything until it is required, improving your Minecraft start times. | [astei](https://github.com/astei) |
| [DashLoader](https://modrinth.com/mod/dashloader) | DashLoader caches all of Minecraft's contents to load the game much faster and provide insanely quick reloads. | [alphaqu](https://github.com/alphaqu) |
| [Enhanced Block Entities](https://modrinth.com/mod/ebe) | Improves block entities by making them used baked models instead, allowing for better performance, visuals (via better smoothlighting), and better resource pack customizability. | [FoundationGames](https://github.com/FoundationGames) |
| [FerriteCore](https://modrinth.com/mod/ferrite-core/versions) | Helps reduce the amount of memory the game takes up. This may make a big difference for larger modpacks as well. | [malte0811](https://github.com/malte0811) |
| [Entity Culling](https://modrinth.com/mod/entityculling) | Culls entities that you cannot see, increasing FPS. While Sodium already does this, this mod is much more thorough in which entities can be culled. | [tr7zw](https://github.com/tr7zw) |
| [More Culling](https://modrinth.com/mod/moreculling) | Cull's more block faces not already culled by Sodium. Can provide a massive performance boost when many of these blocks are in view. | [fxmorin](https://github.com/fxmorin) |
| [ImmediatelyFast](https://modrinth.com/mod/immediatelyfast) | Improves the immediate mode rendering performance. | [RaphiMC](https://github.com/RaphiMC) |
| [Memory Leak Fix](https://modrinth.com/mod/memoryleakfix) | Fixes multiple memory leaks found in the game to prevent excessive memory use. | [fxmorin](https://github.com/fxmorin) | 
| [Dynamic FPS](https://modrinth.com/mod/dynamic-fps) | Reduces your FPS when tabbed out of the game, therefore reducing your system load. | [juliand665](https://github.com/juliand665) |
| [Lazy Language Loader](https://modrinth.com/mod/lazy-language-loader) | Improves loading times when changing your language in game by only reloading the required resources. | [chachy](https://github.com/ChachyDev) |
| [Sodium Extra](https://modrinth.com/mod/sodium-extra) | Allows you to half the resolution on Apple's Retina displays and also adds most of OptiFine's performance features such as toggles for animations, particles, rain/snow, clouds, sky and biome colors, and more, as well as some custom ones. | [FlashyReese](https://github.com/FlashyReese) |
| [Recipe Cache](https://www.curseforge.com/minecraft/mc-mods/recipe-cache) | Caches recipes to reduce lag when crafting or smelting many items. | [biom4st3r](https://gitlab.com/biom4st3r) |
| [Debugify](https://modrinth.com/mod/debugify) | Fixes several bugs in Minecraft, including a few which can effect performance. This will fix lag spikes when crossing chunks and when clicking on links or the resource pack folder button, reduces time it takes to load into a world, and fixes entity collision checks being needlessly calculated client side. | [isXander](https://github.com/isXander) |
| [Audio Engine Tweaks](https://modrinth.com/mod/audio-engine-tweaks) | Fixes the sound pool overloading, allowing for sounds to continue playing at all time and without log spam. | [mattymatty97](https://github.com/mattymatty97) |
| [FastAnim](https://modrinth.com/mod/fastanim) | FastAnim reduces entity animation calculations by storing known and easy values. | [Lunade_](https://github.com/AViewFromTheTop) |

### Other Performance Mods

These are other performance mods that one may prefer to use, but are not required. It is neither recommended or unrecommended, and is up to the player to decide given their use-case.

| Mod | Description | Author | Incompatibilities |
| --- | --- | --- | --- |
| [Phosphor](https://modrinth.com/mod/phosphor) | Phosphor is similar to Starlight in that they both speed up the light engine. However, Phosphor ensures full vanilla parity as compared to Starlight, which may break things such as light suppression. Use Phosphor instead of Starlight if you are looking for vanilla parity at the expense of being slightly slower. Starlight may also cause stuttering on some machines, in which case you should use Phosphor instead. | [CaffeineMC](https://github.com/CaffeineMC) | Starlight |
| [Skip Transitions (No 1.19 Yet)](https://modrinth.com/mod/skip-transitions) | Removes transitions such as the fading animation that Mojang added between their splash screens. This may provide a smoother experience if the fade is choppy on a low end machine or allow people to access certain menus quicker if they do not like the small wait time. | [TrufflezMC](https://github.com/trufflezmc) |
| [Krypton](https://modrinth.com/mod/krypton) | This mod is bannable on Hypixel and most likely other servers. Although it is probably not detectable, it is still against Hypixel's rules and the mod developer does not recommend using it on Hypixel. However, this mod works great for private servers. Krypton optimizes network stacking and entity tracking, as well as other micro-optimizations. | [astei](https://github.com/astei) |

### Recommended

These are mods that I personally recommend due to their usefulness. While they may not boost performance, they are mostly quality of life mods meant to better your experience.

| Mod | Description | Author | Incompatibilities |
| --- | --- | --- | --- |
| [Item Model Fix](https://modrinth.com/mod/item-model-fix) | Fixes the gaps you see on items when holding them. This makes for a much more pleasant experience for most resourcepacks, including both defaults. | [Pepper_Bell](https://github.com/PepperCode1) |
| [Borderless Mining](https://modrinth.com/mod/borderless-mining) | Borderless Fullscreen for Minecraft. This makes the game not minimize when you tab out. | [comp500](https://github.com/comp500) |
| [Recursive Reources](https://modrinth.com/mod/recursiveresources) | Resource Pack Organizer but ported to Fabric and with more features. It allows you to sort resource packs into folders, as well as search for them using a search bar. It also lets you change how resourcepacks are ordered.
| [Smooth Scrolling Everywhere](https://www.curseforge.com/minecraft/mc-mods/smooth-scrolling-everywhere-fabric) | Makes the scrolling in all menus smoother. (MAY HAVE A PROBLEM WITH CONFIG RESETS) | [Shedaniel](https://github.com/shedaniel) |
| [Controlling](https://www.curseforge.com/minecraft/mc-mods/controlling) | Completely revamps Minecraft's controls menu, making it much easier to navigate and change keys, letting you search and more easily find conflicting keybinds. | [Jaredllll08](https://github.com/jaredlll08) |
| [Better Recipe Book](https://www.modrinth.com/mod/brb) | Brings many QOL improvements to the current recipe book, making it much more useful for different scenarios. | [marshmallow](https://github.com/mrshmllow) |
| [Inspecio](https://modrinth.com/mod/inspecio) | Adds more information to tooltips for many items in the game, including shulker boxes. It is very customizable with a large set of config options. | [Queerbic](https://github.com/Queerbric) |
| [CompactChat](https://modrinth.com/mod/compactchat) | Compacts duplicate chat messages to help clean your chat. It also lets you increase your chat history length. | [cbyrne](https://github.com/cbyrneee) |
| [Gamma Utils](https://modrinth.com/mod/gamma-utils) | Fully configurable gamma utility mod. Fullbright but for Fabric. | [Sjouwer](https://github.com/Sjouwer) |

### Other Cool Mods

These are mods that are more dependant on personal preference than importance.

| Mod | Description | Author | Incompatibilities |
| --- | --- | --- | --- |
| [Cosmetica](https://modrinth.com/mod/cosmetica) | Adds cosmetics to your game completely for free! Also supports showing cosmetics from other clients and mods! | [Cosmetica-cc](https://github.com/Cosmetica-cc)
| [3D Skin Layers](https://modrinth.com/mod/3dskinlayers) | Makes the outer layer of skins 3D. Very customizable and lets you adjust distance that 3D renders for performance. | [tr7zw](https://github.com/tr7zw) |
| [Easeify](https://modrinth.com/mod/easeify) | Easeify is a QOL mod with many features. Check out the projects README for more information. | [Polyfrost](https://github.com/Polyfrost) |
| [Midnight Controls](https://modrinth.com/mod/midnightcontrols) | Allows you to easily play Minecraft with a controller. | [TeamMidnightDust](https://github.com/TeamMidnightDust/MidnightControls) |
| [CleanView](https://www.curseforge.com/minecraft/mc-mods/cleanview-fabric) | Prevents self particles from appearing on your screen. | [LianMI](https://github.com/zlainsama) |
| [Color Me Outlines](https://modrinth.com/mod/color-me-outlines) | Color Me Outlines is a close equivalent to 1.8's block overlay, allowing you to customize the outline when looking at blocks. | [LordDeatHunter](https://github.com/LordDeatHunter) |
| [HitBox+](https://modrinth.com/mod/hitboxplus) | HitBox+ allows you to customize hitboxes, similar to 1.8 mods and clients. | [(PingIsFun)[https://github.com/PingIsFun] |
| [Slight GUI Modifications](https://www.curseforge.com/minecraft/mc-mods/slight-gui-modifications) | Adds animations to many GUI elements. | [Shedaniel](https://github.com/shedaniel) |
| [Colored Lights (No 1.19 Yet)](https://modrinth.com/mod/colored-lights) | Adds colored lighting to Minecraft with its colors completely customizable via resource pack. | [Gegy](https://github.com/Gegy) | Sodium |
| [Blur](https://modrinth.com/mod/blur-fabric) | Creates a nice blur effect when in menus and is completely customizable. | [Motschen](https://github.com/Motschen) | Rainbowify |
| [Rainbowify](https://modrinth.com/mod/rainbowify) | Replaces the dark GUI backgrounds with a smooth rainbow one. | [Lennox](https://github.com/officialLennox) | Blur |
| [WaveyCapes](https://modrinth.com/mod/wavey-capes) | Breaks your cape into smaller sections to make its movement more fluid. Looks great with the new migration capes. | [tr7zw](https://github.com/tr7zw) |
| [Perspektive](https://modrinth.com/mod/perspektive) | A simple 360 degrees perspective mod that lets you move the camera without moving your player's direction. | [r0yzer](https://github.com/r0yzer) |
| [EvergreenHUD (No 1.19 Yet)](https://modrinth.com/mod/evergreenhud) | Adds many useful HUD elements to your screen with an easy to use in game config. | [isXander](https://github.com/isXander) |
| [BetterF3](https://modrinth.com/mod/betterf3) | Replaces Minecraft's original debug HUD with a highly customizable, more human-readable HUD. You can customize colors, position, add spacings, and more. | [cominixo](https://github.com/cominixo) |
| [TNTTime (No 1.19 Yet)](https://modrinth.com/mod/tnttime) | Displays time left to the TNT explosion above primed TNT. | [Simon](https://github.com/shateq) |
| [Advancement Info](https://modrinth.com/mod/advancementinfo) | Makes the advancement menu fit your entire screen, which could make it easier to navigate the menu. | [Giselbaer](https://github.com/gbl)
| [AppleSkin](https://modrinth.com/mod/appleskin/) | Lets you know how much a food will restore your hunger bar. | [Ryan Liptak](https://github.com/squeek502) |
| [Horse Stats Vanilla](https://github.com/d4rkm0nkey/HorseStatsVanilla/releases/latest) | Adds the stats of your horse in your horse/donkey inventory HUD, making it easy to see the perks of your horses and donkeys. | [d4m0n](https://github.com/d4rkm0nkey) |
| [Better Mount HUD](https://modrinth.com/mod/better-mount-hud) | Makes some important HUD modules visible when riding a mount. | [Lortseam_](https://www.curseforge.com/members/lortseam_/projects) |
| [Clear Despawn](https://modrinth.com/mod/cleardespawn) | Clear Despawn makes it more obvious on which items are about to despawn by making them blink exponentially faster after a certain time. | [StrikerRockers](https://github.com/StrikerRockers-Mods) |
| [Litematica](https://www.curseforge.com/minecraft/mc-mods/litematica) | A schematic mod that allows you to import schematics of builds. | [Matti Ruohonen](https://github.com/maruohon) |
| [MiniHUD](https://www.curseforge.com/minecraft/mc-mods/minihud) | A customizable HUD that allows displaying various information on your screen as well as beneficial overlay renders. | [Matti Ruohonen](https://github.com/maruohon) |
| [Clear Skies](https://modrinth.com/mod/clear-skies) | Removes fog color banding on skybox. | [grondag](https://github.com/grondag) |
| [Extended Clouds](https://modrinth.com/mod/extended-clouds) | Changes cloud render distance to be same as your set render distance. | [alphaqu](https://github.com/alphaqu) |
| [Why Am I on Fire? (No 1.19 Yet)](https://modrinth.com/mod/why-am-i-on-fire) | Removes the fire overlay when you have fire resistance or are in creative mode. | [Elivers](https://github.com/Ellivers) |
| [Sound Physics (No 1.19 Yet)](https://modrinth.com/mod/soundphysics) | Makes sounds much more realistic, adding reverb, attenuation, and absorption. | [vlad2305m](https://github.com/vlad2305m) & [thedocruby](https://github.com/thedocruby) | Sound Physics Remastered |
| [Universal Chat](https://www.curseforge.com/minecraft/mc-mods/universalchat) | Translates chat messages to different languages. | [mineblock11](https://github.com/mineblock11) |
| [Screencapper](https://modrinth.com/mod/screencapper) | Improves the way you share and view screenshots. | [Deftu](https://github.com/Deftu) |

### OptiFine Replacements

As OptiFine is no longer recommended, here are some replacements for many of it's features. Please note that some mods that have been listed in the above categories may be repeated here.

#### Features

Features that OptiFine provides that are not resource pack related.

| Mod | Description | Author | Incompatibilities |
| --- | --- | --- | --- |
| [Zoomify](https://modrinth.com/mod/zoomify) | Zoom. More customizable than OptiFine's. | [isXander](https://github.com/isXander) |
| [Bobby](https://modrinth.com/mod/bobby) | Higher render distances. More customizable than OptiFine's. | [Johni0702](https://github.com/Johni0702) |
| [LambDynamicLights](https://modrinth.com/mod/lambdynamiclights) | Dynamic lights. More customizable than OptiFine. | [LambdAurora](https://github.com/LambdAurora) |
| [LambdaBetterGrass](https://modrinth.com/mod/lambdabettergrass) | Better grass and better snow. More customizable than OptiFine. | [LambdAurora](https://github.com/LambdAurora) |
| [Cull Less Leaves](https://modrinth.com/mod/cull-less-leaves) | Smart leaves. | [isXander](https://github.com/isXander) |
| [Fabrishot](https://modrinth.com/mod/fabrishot) | Higher resolution Screenshots. More customizable than OptiFine. | [ramidzkh](https://modrinth.com/user/z0r5biKh) |

#### Resource Packs

Resource pack features that OptiFine has. Not all support the OptiFine format.

| Mod | Description | Author | Incompatibilities |
| --- | --- | --- | --- |
| [Custom Splash Screen (No 1.19 Yet)](https://modrinth.com/mod/custom-splash-screen) | Custom loading screen colors. Does not support OptiFine format. | [MidnightDust](https://github.com/TeamMidnightDust) |
| [FabricSkyboxes](https://modrinth.com/mod/fabricskyboxes) | Custom sky. Does not support OptiFine format. | [AMereBagatelle](https://modrinth.com/user/ifLBWnLs) |
| [Continuity](https://modrinth.com/mod/continuity) | Connected texture models (CTM) and emmisive textures. Supports OptiFine format. | [Pepper_Bell](https://github.com/PepperCode1) |
| [Animatica](https://modrinth.com/mod/animatica) | Animated textures. Supports OptiFine format. | [FoundationGames](https://github.com/FoundationGames) |
| [OptiGUI](https://modrinth.com/mod/optigui) | GUI/Container textures. Supports OptiFine format. | [opekope2](https://github.com/opekope2) |
| [Semitranslucency Fix](https://modrinth.com/mod/semitranslucency) | Fixes semitranslucent textures. Honestly have no clue if OptiFine does this but it probably does idk. | [ruvaldk](https://github.com/ruvaldak) |
| [CIT Resewn](https://modrinth.com/mod/cit-resewn) | Custom item textures. Supports OptiFine format. | [SHsuperCM](https://github.com/SHsuperCM) |
| [Colormatic](https://github.com/kvverti/colormatic/releases/latest) | Custom colors. Does not support OptiFine format. | [Thalia](https://github.com/kvverti) |
| [Custom Entity Models](https://modrinth.com/mod/cem) | Custom entity models. Supports OptiFine format. | [dorianpb](https://github.com/dorianpb) |
| [Entity Texture Features](https://modrinth.com/mod/entitytexturefeatures) | Random and emissive entity textures. Supports OptiFine format. | [Traben](https://github.com/btrab1) |
| [JsonEM](https://modrinth.com/mod/jsonem) | Custom JSON Entity Models. Does not support OptiFine format. | [FoundationGames](https://github.com/FoundationGames) |
| [Puzzle](https://modrinth.com/mod/puzzle) | Adds custom splash screens, better logo blending, unlimited model rotations, and bigger custom models. Incorporates a platform to configure OptiFine replacements from other mods. Supports OptiFine format. | [PuzzleMC](https://github.com/PuzzleMC) |
| [MCPatcherPatcher++](https://modrinth.com/mod/mcpppp) | Converts from OptiFine format to newer formats. | [supsm](https://github.com/supsm) |

### Internal Shader

If you are one of those weirdos who uses internal shaders (you shouldn't btw), here's a mod that does the same thing.

| Mod | Description | Author | Incompatibilities |
| --- | --- | --- | --- |
| [Simply No Shading](https://modrinth.com/mod/simply-no-shading) | Internal Shaders | [StartsMercury](https://github.com/StartsMercury) |

### Unrecommended Mods

These are mods that are too experimental or unstable that I do not recommend using unless you know what you are doing. Please note that some of these mods will continue to be improved upon over time and may eventually be added to the above lists.

#### May Eventually Be Supported

| Mod | Reasoning | Author |
| --- | --- | --- |
| C2ME | C2ME is an experimental mod that attempts to multithread chunk generation, I/O, and loading. It is deemed not production ready by the authors and may corrupt worlds or cause other issues. It also comes with its own list of incompatible mods. If you decide to use it, remember to make backups. | [RelativityMC](https://github.com/RelativityMC) |
| VMP (Very Many Players) | VMP attempts to alleviate the strain on servers when there are a large amount of players. It is still in early development and may cause issues according to the authors, who also made C2ME. If you decide to use it, remember to make backups. | [RelativityMC](https://github.com/RelativityMC) |

#### Will Never Be Supported

| Mod | Reasoning | Author |
| --- | --- | --- |
| Not Enough Crashes | NEC regularly causes the game to be in an invalid state and blames the wrong mods for crashes, making it harder for mod devs to debug. | [natanfudge](https://github.com/natanfudge) |
| Better Beds | BetterBeds has been replaced by Enhanced Block Entities. | [Motschen](https://github.com/Motschen) |
| Iris Starline | The Iris Starline fork was meant to provide a shaders option menu before Iris created their own much improved version. This fork serves no purpose to users. | [HyperCubeMC](https://github.com/HyperCubeMC) |
| Sound Physics Remastered | This remastered version is based off an old version of the original mod. The original has now been updated to surpass this edit and it is recommended to use the original over this now. | [henkelmax](https://github.com/henkelmax) |
| Smooth Boot | While Smooth Boot does great at decreasing startup time, it is no match for LazyDFU and DashLoader. Smooth Boot will also cause a decrease in performance for several minutes after startup according to some reports. | [UltimateBoomer](https://github.com/UltimateBoomer) |
| FastOpenLinksAndFolders | Superseded by Debugify. | [Altrisi](https://github.com/altrisi) |
| ForgetMeChunk | Superseded by Debugify. | [Breadloaf](https://github.com/mjwells2002) |
| ToolTipFix | Superseded by Debugify. | [kyrptonaught](https://github.com/kyrptonaught) |

# Notes

Join my [Discord server](https://inv.wtf/micro) for news regarding the development of this repository!

If you would like to contribute, please make a PR.  
Some notes:
- Leave your name and GitHub link in the contributors credits section in alphabetical order, even for a tiny change
- Please try to use Modrinth or GitHub over CurseForge when possible (Modrinth is the preferred platform)
- Please use a GitHub link instead of a Modrinth/CurseForge link for Author credit when possible
    - If the GitHub profile is an organization, use that instead of one of the owners / person credited on Modrinth/CurseForge
- Make sure that the option to allow me to make changes to your PR is enabled

## Contributors

- [BobIsMyManager](https://github.com/BobIsMyManager)
- [glai](https://github.com/glaicodes)
- [karmette](https://github.com/karmette)
- [Moisty](https://github.com/Mqisty)
- [nacrt](https://github.com/nacrt)
- [NoPro2024](https://github.com/NoPro2024)
- [osfanbuff](https://github.com/osfanbuff63)
- [Lisena](https://github.com/Lisenaaaa)
- [Lulonaut](https://github.com/Lulonaut)
- [Wyvest](https://github.com/Wyvest)

And a special thanks to [LambdAurora](https://gist.github.com/LambdAurora) for her own [OptiFine Alternatives](https://lambdaurora.dev/optifine_alternatives/) gist that first helped me start using Fabric and helped with inspiration and mod finding for this list.
