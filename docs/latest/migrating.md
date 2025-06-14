# Migrating to Latest 

This is a comprehensive guide on how to download Fabric and mods for it. It also provides direct links to many mods that you may find useful.

## Introduction

If you want more information on Fabric, why Forge/OptiFine are not recommended, or need help downloading Fabric and mods for it, click on the `Introduction` drop down below. If you are just here to see the mods list, continue to the next section.

??? note "Introduction"

    ### The Situation

    So, you've been playing 1.8.9 for the past [9 years](https://howoldisminecraft189.today) and are ready to see what 1.21 has to offer. Your first thought may be to download and install Forge and then add OptiFine as a mod, but this could not be further from the best choice. As Mojang has been rolling out releases, they've also been decreasing performance with every version, and neither Forge nor OptiFine are really able to bring back even a speck of that performance we see in 1.12 and below. However, another mod loader, Fabric, which is lightweight and easier to develop for, has created an amazing community in which many of its members focus on helping optimize the game to its greatest potential.

    ### Why no longer OptiFine?

    OptiFine no longer provides the benefit that it once did on older versions of the game. As the years have gone by and Minecraft's code has changed, OptiFine has been continuing to completely overwrite major parts of Minecraft's code. Because OptiFine is closed source, it has become increasingly harder for modders to provide OptiFine compatibility. OptiFine also uses outdated formats for many of its features, including MCPatcher and its confusing and outdated settings menu. Many members in the Fabric community have taken it upon themselves to create better performance enhancing mods which surpass OptiFine, as well as provide alternatives to many of OptiFine's iconic features.

    While there is a Fabric compatibility layer for OptiFine known as OptiFabric, it is unsupported by many of the mods on the list, with some outright preventing the game from loading if OptiFabric is present. Therefore, consider all mods in this list to be incompatible with OptiFabric.

    ### Why no longer Forge?

    Forge has always been less than ideal for performance due to its large overhead for server-sided modding, which is not necessary for users wishing for a vanilla compatible experience. Fabric on the other hand is extremely lightweight and is practically identical to vanilla. It's also considered to be much easier to make mods for.

    Unlike Fabric, which aims to modify vanilla as little as possible, Forge makes a lot of changes that simply are not beneficial for our usecases. For example, for several months and spanning several Minecraft versions, there was a [bug in Forge](https://github.com/MinecraftForge/MinecraftForge/issues/9309) that gave the player 4-5 block reach in survival mode, effectively banning every Forge player playing on any server with an anticheat at that time. Due to Fabric's goal of being as uninvasive as possible, issues like this won't arise with Fabric Loader, and if they did, would be fixed much quicker.

    ### Installing Fabric

    Due to many issues with the official Minecraft launcher, we will not be using it. We will be using the ModrinthApp instead, which is a much improved launcher that has many more features than the official Minecraft launcher and is made with mods in mind.

    Install the app from the [Modrinth page](https://modrinth.com/app) and continue on with the installation. The Modrinth app should walk you through how to log in, create profiles, and install mods.

    Once this is completed and you are back at the main home page, press the create profile button on the bottom left (the green plus sign). Select any icon and give it any name you want, set the loader to Fabric, and select the game version to 1.21.

    ### Downloading and Installing Mods for Fabric

    This list currently consists of three different sources for mod downloads: Modrinth, GitHub, and CurseForge. This section will explain how to download mods from each of them.

    #### Automatic Installation:
    
    - You can simply click on the instance go to the Content tab and press the "Add content" button in the top right to search Modrinth directly inside the launcher.

    - GitHub and CurseForge mods will require manual installation. The Content tab has a dropdown next to the Add content button to add from file. Use that to add the mods you have downloaded.

    #### Manual Download

    - Modrinth:
        - On the mod's page, click on the `Versions` tab. From there, you can see all versions of the mod. Make sure you download the correct one based on the Minecraft version and mod loader, click on the download icon for the newest version of the mod that fits both previous criteria.

    - GitHub:
        - For your convenience, all GitHub links lead directly to the latest version of the mod. From here, click on the `Assets` drop down if needed, then download the jar that does not include `-sources` or `-dev` in the name.
            - If a link does not redirect you to the latest version but rather the main page, on the right side of the page, you should find a tag icon with the latest version.

    - CurseForge:
        - Click on the `Files` tab. Look for the versions of the mod with the Minecraft version you desire and is for the Fabric mod loader, and download the latest one. You can also press the `View All` button, then sort by mod loader or Minecraft version to make finding the correct jar easier.

    ### Still Need Help?

    Feel free to join my [Discord server](https://discord.gg/rejfv9kFJj) for any help downloading Fabric, its mods, or general questions about them.
    
## Mods

### Note about Dependencies

Dependencies are smaller mods that main mods rely on to function. If you are using Modrinth or Prism launcher, these should be automatically downloaded for you when you download mods within the launcher, and you don't need to worry about it. Please use one of these launchers to manage dependencies for you!

### Performance

These are mods that are needed for playing the latest versions of Minecraft at a reasonable FPS. These will also help decrease frame times, hopefully eliminating spikes or stuttering.

| Mod | Description | Author |Incompatabilities | Notes |
| --- | --- | --- | --- | --- |
| [Sodium](https://modrinth.com/mod/sodium) | An all around performance mod, Sodium allows users to play the latest versions of Minecraft with high FPS, completely outperforming OptiFine, with some users seeing up to 8x their vanilla frames. Sodium also drastically improve visuals, providing a much better gameplay experience. | [CaffeineMC](https://github.com/CaffeineMC) |
| [Iris](https://modrinth.com/mod/iris) | A shader loader that allows users to load up their favorite OptiFine shaderpacks, but with much higher FPS. Iris also provides performance enhancements when not using shaders, making it great for all users. | [Iris Team](https://github.com/IrisShaders) | 
| [Lithium](https://modrinth.com/mod/lithium) | Helps improve the performance of many vanilla systems without changing their mechanics. | [CaffeineMC](https://github.com/CaffeineMC) |
| [Exordium](https://modrinth.com/mod/exordium) (No 1.21.5 Yet) | Caps the FPS of certain HUD elements that do not need to be updated every frame. | [tr7zw](https://github.com/tr7zw) | | May break some HUD elements from other mods. |
| [Enhanced Block Entities](https://modrinth.com/mod/ebe) (No 1.21.5 Yet) | Improves block entities by making them used baked models instead, allowing for better performance, visuals (via better smoothlighting), and better resource pack customizability. | [FoundationGames](https://github.com/FoundationGames) |
| [FerriteCore](https://modrinth.com/mod/ferrite-core) | Helps reduce the amount of memory the game takes up. This may make a big difference for larger modpacks as well. | [malte0811](https://github.com/malte0811) |
| [Entity Culling](https://modrinth.com/mod/entityculling) | Culls entities that you cannot see, increasing FPS. While Sodium already does this, this mod is much more thorough in which entities can be culled. | [tr7zw](https://github.com/tr7zw) |
| [ImmediatelyFast](https://modrinth.com/mod/immediatelyfast) | Improves the immediate mode rendering performance. | [RaphiMC](https://github.com/RaphiMC) |
| [ModernFix](https://modrinth.com/mod/modernfix) (No 1.21.5 Yet) | ModernFix is an all-in-one mod that improves performance, reduces memory usage, and fixes many bugs in modern Minecraft versions without majorly compromising the game experience. | [embeddedt](https://github.com/embeddedt) |
| [Dynamic FPS](https://modrinth.com/mod/dynamic-fps) | Reduces your FPS when tabbed out of the game, therefore reducing your system load. | [juliand665](https://github.com/juliand665) |
| [Lazy Language Loader](https://modrinth.com/mod/lazy-language-loader) | Improves loading times when changing your language in game by only reloading the required resources. | [chachy](https://github.com/ChachyDev) |
| [Sodium Extra](https://modrinth.com/mod/sodium-extra) | Allows you to half the resolution on Apple's Retina displays and also adds most of OptiFine's performance features such as toggles for animations, particles, rain/snow, clouds, sky and biome colors, and more, as well as some custom ones. | [FlashyReese](https://github.com/FlashyReese) |
| [Debugify](https://modrinth.com/mod/debugify) | Fixes several bugs in Minecraft, including a few which can effect performance. This will fix lag spikes when crossing chunks and when clicking on links or the resource pack folder button, reduces time it takes to load into a world, and fixes entity collision checks being needlessly calculated client side. | [isXander](https://github.com/isXander) |
| [Audio Engine Tweaks](https://modrinth.com/mod/audio-engine-tweaks) | Fixes the sound pool overloading, allowing for sounds to continue playing at all time and without log spam. | [mattymatty97](https://github.com/mattymatty97) |
| [Ksyxis](https://modrinth.com/mod/ksyxis) | Reduces world loading times. | [VidTu](https://github.com/VidTu) |
| [FastQuit](https://modrinth.com/mod/fastquit) | Allows you to go back to the title screen while the world is still loading or saving. It is done in a way that prevents world corruption. | [KingContaria](https://github.com/KingContaria) |
| [Noxesium](https://modrinth.com/mod/noxesium) | Contains several smaller performance improvements and also has many visual bug fixes for the MCCI server. | [Noxcrew](https://github.com/Noxcrew) |
| [Remove Reloading Screen](https://modrinth.com/mod/rrls) | Allows you to access other parts of the game by removing the reload screen except for the progress bar. | [dima_dencep](https://github.com/dimadencep) |
| [C2ME](https://modrinth.com/mod/c2me-fabric) | C2ME is an experimental mod that attempts to multithread chunk generation, I/O, and loading. | [RelativityMC](https://github.com/RelativityMC) |
| [Very Many Players](https://modrinth.com/mod/vmp-fabric) | VMP attempts to alleviate the strain on servers when there are a large amount of players. | [RelativityMC](https://github.com/RelativityMC) |
| [Noisium](https://modrinth.com/mod/noisium) | Optimizes world generation when generating new chunks. | [Steveplays](https://github.com/Steveplays28) |
| [Particle Core](https://modrinth.com/mod/particle-core) | Several optimizations to particles in Minecraft and customization of particle rendering, i.e., being able to turn them on/off individually and putting them in a reduced state. | [fzzyhmstrs](https://github.com/fzzyhmstrs) |
| [AsyncParticles](https://modrinth.com/mod/asyncparticles) | Improves particle performance by implementing async particle rendering and ticking. | [Harvey Husky](https://github.com/Harveykang) |
| [Force Close Loading Screen](https://modrinth.com/mod/forcecloseworldloadingscreen) | Instantly closes the loading terrain screen on world changing and drastically reduces the resource pack loading screen duration. | [kennytv](https://github.com/kennytv) |
| [BadOptimizations](https://modrinth.com/mod/badoptimizations) | A collection of micro-optimizations. | [Thosea](https://github.com/imthosea) |
| [Structure Layout Optimizer](https://modrinth.com/mod/structure-layout-optimizer) | Attempts to optimize the generation of Jigsaw Structures and NBT pieces. | [TelepathicGrunt](https://github.com/TelepathicGrunt) |

### Other Performance Mods

These are other performance mods that one may prefer to use, but are not required. It is neither recommended or unrecommended, and is up to the player to decide given their use-case.

| Mod | Description | Author | Incompatabilities | Notes |
| --- | --- | --- | --- | --- |
| [Nvidium](https://modrinth.com/mod/nvidium) | Nvidium uses NVIDIA only OpenGL extensions to greatly improve the game's performance. This mod will not work on AMD. It has a few graphical glitches and could lead to crashes, as the mod is still in beta and not considered stable yet. The mod will also disable itself whenever Iris shaders are enabled or if the required OpenGL extensions are not available. | [MCRcortex](https://github.com/MCRcortex) | | Chunks won't fade when using [Chunks Fade In](https://modrinth.com/mod/chunks-fade-in). |
| [Fadeless](https://modrinth.com/mod/fadeless) | Removes transitions such as the fading animation that Mojang added between their splash screens. This may provide a smoother experience if the fade is choppy on a low end machine or allow people to access certain menus quicker if they do not like the small wait time. This mod is made partially redundant by Remove Loading Screen. | [DerpDerpling](https://github.com/DerpDerpling) & [UltimateBoomer](https://github.com/UltimateBoomer) |
| [Krypton](https://modrinth.com/mod/krypton) | This mod is bannable on Hypixel and most likely other servers. Although it is probably not detectable, it is still against Hypixel's rules and the mod developer does not recommend using it on Hypixel. However, this mod works great for private servers. Krypton optimizes network stacking and entity tracking, as well as other micro-optimizations. | [astei](https://github.com/astei) |

### Recommended

These are mods that I personally recommend due to their usefulness. While they may not boost performance, they are mostly quality of life mods meant to better your experience.

| Mod | Description | Author |Incompatabilities | Notes |
| --- | --- | --- | --- | --- |
| [No Chat Reports](https://modrinth.com/mod/no-chat-reports) | Removes cryptographic signatures from chat messages, making it harder to get chat reported. | [Aizistral](https://github.com/Aizistral-Studios) |
| [Amecs Reborn](https://modrinth.com/mod/amecs-reborn) | Allows you to use modifiers for keybinds. For example, you can set keybinds to Ctrl/Shift/Alt/Super + key. | [Nova-Committee](https://github.com/MisterCheezeCake) |
| [Model Gap Fix](https://modrinth.com/mod/modelfix) | Fixes the gaps you see on items when holding them as well as 3D blocks. This makes for a much more pleasant experience for most resourcepacks, including both defaults. | [MehVahdJukaar](https://github.com/MehVahdJukaar) |
| [Cubes Without Borders](https://modrinth.com/mod/cubes-without-borders) | Borderless Fullscreen for Minecraft. This makes the game not minimize when you tab out. | [Kir-Antipov](https://github.com/Kir-Antipov) |
| [Recursive Resources](https://modrinth.com/mod/recursiveresources) | Resource Pack Organizer but ported to Fabric and with more features. It allows you to sort resource packs into folders, as well as search for them using a search bar. It also lets you change how resourcepacks are ordered.
| [Smooth Scrolling Refurbished](https://modrinth.com/mod/smooth-scrolling-refurbished) | Makes the scrolling in all menus smoother. | [JustAlittleWolf](https://github.com/JustAlittleWolf) |
| [Controlling](https://modrinth.com/mod/controlling) | Completely revamps Minecraft's controls menu, making it much easier to navigate and change keys, letting you search and more easily find conflicting keybinds. | [Jaredllll08](https://github.com/jaredlll08) |
| [Chat Patches](https://modrinth.com/mod/chatpatches) | Adds several QOL features to Minecraft's chat to make it more usable. | [mrbuilder1961](https://github.com/mrbuilder1961) |
| [MixinTrace](https://modrinth.com/mod/mixintrace) | Makes it easier for mod developers to debug crash reports. | [comp500](https://github.com/comp500) |
| [Adaptive Tooltips](https://modrinth.com/mod/adaptive-tooltips) (No 1.21.4 Yet) | Makes tooltips more readable by preventing them from going off screen and allowing for tooltip scrolling, as well as more customization options such as custom transparency. | [isXander](https://github.com/isXander) |
| [Persistent Stuff](https://modrinth.com/mod/persistent-stuff) | Saves your toggle sprint (sprinting/walking), hitboxes' (enabled/disabled), chunk borders' (enabled/disabled) states across Minecraft restarts. Never toggle these at startup again. | [Andy Russo](https://github.com/AndyRusso) | | | The mod author has not updated the supported Minecraft versions on the Modrinth page, but it should work with no issues regardless. |
| [Log Cleaner](https://modrinth.com/mod/log-cleaner) | Automatically deletes old logs to clear up storage space. | [Altrisi](https://github.com/altrisi) | | | (Probably) works on 1.21 despite not being updated to it. |
| [Better Selection](https://modrinth.com/mod/better-selection) | Makes it easier to select text by allowing mouse selection and Ctrl + ← and Ctrl + →. | [MDLC01](https://github.com/MDLC01) |
| [Auto ReAuth](https://modrinth.com/mod/auto-reauth) | Automatically reauthenticates your session when you are not logged in correctly. | [connorslade](https://github.com/connorslade) |
| [In-Game Account Switcher](https://modrinth.com/mod/in-game-account-switcher) | Adds an in game account switcher that lets you switch accounts without having to restart the game. | [The-Fireplace](https://github.com/The-Fireplace) |
| [Smooth Skies](https://modrinth.com/mod/smooth-skies) | Smooths out the skybox colors on far render distances. This will fix the skybox breaking with Nvidium or similar. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Better Mipmaps](https://modrinth.com/mod/better-mipmaps) | Unlocks mipmap levels higher than 4 to reduce visual arifacts with high resolution resource packs. | [sidit77](https://github.com/sidit77) |
| [Fix Keyboard on Linx](https://modrinth.com/mod/fix-keyboard-on-linux) | Fix several issues regarding key input on Linux. | [Ishland](https://github.com/ishland) | | Works on Linux only, will do nothing for other OS's. Has not been listed as compatible for 1.21+, but it should work with no changes. |
| [MacOS Input Fixes](https://modrinth.com/mod/macos-input-fixes) | Fix several issues regarding key input on MacOS. | [hamarb123](https://github.com/hamarb123) | | Not listed as 1.21.1 compatible, but should work regardless. |
| [Unsafe World Random Access](https://modrinth.com/mod/uwrad) | Detects unsafe off-thread world random access, helping to find causes of "Accessing LegacyRandomSource from multiple threads" crash. | [RelativityMC](https://github.com/RelativityMC) |

### Other Cool Mods

These are mods that are more dependant on personal preference than importance.

| Mod | Description | Author | Incompatabilities | Notes |
| --- | --- | --- | --- | --- |
| [World Host](https://modrinth.com/mod/world-host) | Let's you invite people to your singleplayer worlds! They do not need to have the mod installed for it to work. | [Gaming32](https://github.com/Gaming32) |
| [Cosmetica](https://modrinth.com/mod/cosmetica) (No 1.21.4 Yet) | Adds cosmetics to your game completely for free! Also supports showing cosmetics from other clients and mods! | [Cosmetica-cc](https://github.com/Cosmetica-cc) |
| [3D Skin Layers](https://modrinth.com/mod/3dskinlayers) | Makes the outer layer of skins 3D. Very customizable and lets you adjust distance that 3D renders for performance. | [tr7zw](https://github.com/tr7zw) |
| [BetterGrassify](https://modrinth.com/mod/bettergrassify) | Better grass and snow. | [UltimatChamp](https://github.com/UltimatChamp) & [JayemCeekay](https://github.com/JayemCeekay) |
| [Overlay Tweaks](https://modrinth.com/mod/overlaytweaks) | A small QOL mod that lets you alter vanilla's overlays in small ways. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Nametag Tweaks](https://modrinth.com/mod/nametagtweaks) | Let's you alter the way nametags are rendered, such as background transparency, text shadow, and custom F1 rules. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Scroll Tweaks](https://modrinth.com/mod/scrolltweaks) | Let's you customize Minecraft hotbar scrolling. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Title Tweaks](https://modrinth.com/mod/titletweaks) | Improvements and customization for Minecraft's Titles. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Tab Tweaks](https://modrinth.com/mod/tabtweaks) | Improvements and customization for Minecraft's Tab / Player List HUD. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Crosshair Tweaks](https://modrinth.com/mod/crosshairtweaks) | A small QOL mod that lets you alter the vanilla crosshair in small ways. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Scoreboard Tweaks](https://modrinth.com/mod/scoreboardtweaks) | Client side customization of Minecraft's Scoreboard/Sidebar. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Mount Opacity](https://modrinth.com/mod/mountopacity) | Allows setting custom opacity (transparency) for entities that you are riding | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Dropped Item Tweaks](https://modrinth.com/mod/droppeditemtweaks) | Small changes to the way dropped items render. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Render Tweaks](https://modrinth.com/mod/rendertweaks) | Customization of some in-world visuals. |  [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Inventory Scale](https://modrinth.com/mod/inventoryscale) | Allows customizing your inventory and container scaling independent of GUI scale. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Numerical Enchantments](https://modrinth.com/mod/numerical-enchantments) | Converts roman numerals to arabic numbers in enchantment tooltips to make them easier to read at a glance! No resource pack required. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Sciophobia](https://modrinth.com/mod/sciophobia) | Allows disabling text shadow or only translating it down, globally. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [Custom Block Highlight](https://modrinth.com/mod/custom-block-highlight) | Change how your selected block outline looks, featuring fancy rendering options and animation! | [Tektonikal](https://github.com/Tektonikal) |
| [Chunks Fade In](https://modrinth.com/mod/chunks-fade-in) | Adds a fade-in animation to chunks similar to Bedrock Edition. | [kerudion](https://github.com/kerudion) | Nvidium (chunks don't fade) |
| [Distant Horizons](https://modrinth.com/mod/distanthorizons) | Adds LODs to Minecraft, allowing for much further render distances without a big tank on performance. | [James Seibel](https://gitlab.com/jeseibel) |
| [Controlify](https://modrinth.com/mod/controlify) | Allows you to easily play Minecraft with a controller. | [isXander](https://github.com/isXander) |
| [CleanView](https://github.com/zlainsama/CleanView/releases/latest) | Prevents self particles from appearing on your screen. | [LianMI](https://github.com/zlainsama) |
| [HitBox+](https://modrinth.com/mod/hitboxplus)  | Allows you to customize hitboxes, similar to 1.8 mods and clients. | [PingIsFun](https://github.com/PingIsFun) |
| [Blur+](https://modrinth.com/mod/blur-fabric) | Creates a nice blur effect when in menus and is completely customizable. | [Motschen](https://github.com/Motschen) |
| [WaveyCapes](https://modrinth.com/mod/wavey-capes) | Breaks your cape into smaller sections to make its movement more fluid. Looks great with the new migration capes. | [tr7zw](https://github.com/tr7zw) |
| [Perspektive](https://modrinth.com/mod/perspektive) **(BANNABLE ON HYPIXEL)** | A simple 360 degrees perspective mod that lets you move the camera without moving your player's direction. | [r0yzer](https://github.com/r0yzer) |
| [BetterF3](https://modrinth.com/mod/betterf3) | Replaces Minecraft's original debug HUD with a highly customizable, more human-readable HUD. You can customize colors, position, add spacings, and more. | [cominixo](https://github.com/cominixo) |
| [TNTTime](https://modrinth.com/mod/tnttime) (No 1.21.4 Yet) | Displays time left to the TNT explosion above primed TNT. | [Simon](https://github.com/shateq) |
| [Paginated Advancements & Custom Frames](https://modrinth.com/mod/paginatedadvancements) | Makes the advancement menu fit your entire screen, which could make it easier to navigate the menu. | [DaFuqs](https://github.com/DaFuqs)
| [AppleSkin](https://modrinth.com/mod/appleskin) | Lets you know how much a food will restore your hunger bar. | [Ryan Liptak](https://github.com/squeek502) |
| [Horse Stats Vanilla](https://modrinth.com/mod/horsestatsvanilla) (No 1.21.4 Yet) | Adds the stats of your horse in your horse/donkey inventory HUD, making it easy to see the perks of your horses and donkeys. | [d4m0n](https://github.com/d4rkm0nkey) |
| [Better Mount HUD](https://modrinth.com/mod/better-mount-hud) | Makes some important HUD modules visible when riding a mount. | [Lortseam](https://github.com/Lortseam) |
| [Clear Despawn](https://modrinth.com/mod/cleardespawn) | Clear Despawn makes it more obvious on which items are about to despawn by making them blink exponentially faster after a certain time. | [StrikerRockers](https://github.com/StrikerRockers-Mods) |
| [Litematica](https://github.com/sakura-ryoko/litematica/releases/latest) | A schematic mod that allows you to import schematics of builds. | [Matti Ruohonen](https://github.com/maruohon) |
| [MiniHUD](https://github.com/sakura-ryoko/minihud/releases/latest) | A customizable HUD that allows displaying various information on your screen as well as beneficial overlay renders. | [Matti Ruohonen](https://github.com/maruohon) |
| [Sound Physics Remastered](https://modrinth.com/mod/sound-physics-remastered) | Makes sounds much more realistic, adding reverb, attenuation, and absorption. | [vlad2305m](https://github.com/vlad2305m), [thedocruby](https://github.com/thedocruby) & [henkelmax](https://github.com/henkelmax)|
| [Sound Controller](https://modrinth.com/mod/sound-controller) | Provides complete control over the volume of every sound in the game. | [BVengo](https://github.com/BVengo) |
| [Screencapper](https://modrinth.com/mod/screencapper) | Improves the way you share and preview screenshots. | [isXander](https://github.com/isXander) & [Deftu](https://github.com/Deftu) |
| [Snapper](https://modrinth.com/mod/snapper) | An in game screenshot viewer, making it easy to see all your screenshots in game. Also adds the ability to take and view panoramas. | [Spirit Studios](https://github.com/SpiritGameStudios/Snapper) |
| [Better Command Block UI](https://modrinth.com/mod/bettercommandblockui) | Improves the command block user interface by allowing for visual newlining . | [Tectato](https://github.com/Tectato) |
| [Better Statistics Screen](https://modrinth.com/mod/better-stats) | A visual overhaul to the statistics screen, giving useful information in a much more visually appealing format. | [TheCSDev](https://github.com/TheCSDev) |
| [Chat Heads](https://modrinth.com/mod/chat-heads) | Shows a player's head next to their chat message in game. | [dzwdz](https://github.com/dzwdz) |
| [Craftify](https://modrinth.com/mod/craftify) | Shows your currently playing music on your HUD. | [ThatGravyBoat](https://github.com/ThatGravyBoat) |
| [Resourcify](https://modrinth.com/mod/resourcify) | Lets you view, download, and update resource packs from Modrinth all in game. | [DeDiamondPro](https://github.com/DeDiamondPro) |
| [Make Bubbles Pop](https://modrinth.com/mod/make_bubbles_pop) | Improves the look of bubbles in water. | [Tschipcraft](https://github.com/Tschipcraft) |
| [NoRefreshScroll](https://modrinth.com/mod/norefreshscroll) | Stops the multiplayer screen from scrolling to bottom when refreshing. | [Thatsmusic99](https://github.com/Thatsmusic99) |
| [Particle Tweaks](https://modrinth.com/mod/particle-tweaks) | Makes particles look nicerby adding growing/fading effects and water physics. | [Lunade_](https://github.com/AViewFromTheTop) |
| [Particle Rain](https://modrinth.com/mod/particle-rain) | Replaces the rain effect with particles. | [PigCart](https://github.com/PigCart) |
| [SkinShuffle](https://modrinth.com/mod/skinshuffle) | Allows you to change, store, and customize your skins in game. | [mineblock11](https://github.com/mineblock11) |
| [Tiny Item Animations](https://modrinth.com/mod/tiny-item-animations) | Adds a small animation when holding items similar to old console editions of the game. | [Trivaxy](https://github.com/Trivaxy) |
| [Draggable Lists](https://modrinth.com/mod/draggable-lists) | Allows you to drag to order resourcepacks, datapacks, worlds, and servers. | [MrMelon54](https://github.com/MrMelon54) |
| [Highlight](https://modrinth.com/mod/highlight) | Changes hitboxes to allow them to not be axis alligned, making them look much smoother on some blocks. | [Team Resourceful](https://github.com/Team-Resourceful) |
| [Biome Moss](https://modrinth.com/mod/biome-moss) | Improves the look of moss by adding color biome variation. | [TheDarkCoder](https://github.com/TheDarkCoder) |
| [Fluid Void Fading](https://modrinth.com/mod/fluidvoidfading) | Makes liquids like water and lava slowly fade out in the void. Looks great in games like Skyblock, Skyways, or similar. | [DaFuqs](https://github.com/DaFuqs) |
| [Server Pinger Fixer](https://modrinth.com/mod/serverpingerfixer) | Makes server pinging smoother and fixes it breaking when refreshing too many times. | [JustAlittleWolf](https://github.com/JustAlittleWolf) |
| [Axiom](https://modrinth.com/mod/axiom) | An alternative to WorldEdit and VoxelSniper to make building in singleplayer much easier. | [Moulberry](https://github.com/Moulberry) |
| [Sounds](https://modrinth.com/mod/sound) | Adds many more sounds to Minecraft for things that did not previously have sounds. | [mineblock11](https://github.com/mineblock11) |
| [TipTapShow](https://modrinth.com/mod/tiptapshow) | A keystrokes mod for modern fabric. | [Spyxar](https://github.com/Spyxar) |
| [Favorita](https://modrinth.com/mod/favorita) (No 1.21.5 Yet) | A basic item favoriting mod, allowing you to stop yourself from discarding of important items. | [Deftu](https://github.com/Deftu) |
| [SaveMyKeybinds](https://modrinth.com/mod/savemykeybinds) | Allows you to save and load keybind presets. | [MisterCheezeCake](https://github.com/MisterCheezeCake) |
| [Better Elytra Render](https://modrinth.com/mod/better-elytra-render) | Improves the look of elytra by changing its position on the player. | [KGriffon](https://github.com/kgriff0n) |
| [Confirm Disconnect](https://modrinth.com/mod/confirm-disconnect) | Adds a confirmation dialogue before exiting your world/server. | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [No Recipe Book Shift](https://modrinth.com/mod/no-recipe-book-shift) | Prevents the recipe book from shifting the screen! | [Microcontrollers](https://github.com/MicrocontrollersDev) |
| [View Model](https://modrinth.com/mod/no-ones-view-model) | Lets you change the hands positions, similar to Overflow Animations and Dulkir. | [No-One](https://github.com/I-No-oNe) |
| [Dark Loading Screen](https://modrinth.com/mod/dark-loading-screen) | Makes the loading screen darker. Allows for some customization. | [A5b84](https://github.com/A5b84) |
| [Gamma Utils](https://modrinth.com/mod/gamma-utils) | A customizable fullbright mod. | [Sjouwer](https://github.com/Sjouwer) |

### Skyblock Mods

These are mods for Hypixel Skyblock.

| Mod | Description | Author | Incompatabilities | Notes |
| --- | --- | --- | --- | --- |
| [SkyBlock Custom Scoreboard](https://modrinth.com/mod/skyblock-custom-scoreboard) | SkyHanni's CustomScoreboard for modern Hypixel SkyBlock. | [Meowdding](https://github.com/meowdding) |
| [Skyblocker](https://modrinth.com/mod/skyblocker-liap) | A general purpose Hypixel Skyblock utility mod. | [SkyblockerMod Team](https://github.com/SkyblockerMod) |
| [SkyBlock Profile Viewer](https://modrinth.com/mod/skyblock-profile-viewer) | A modern Hypixel SkyBlock profile viewer. | [Meowdding](https://github.com/meowdding) |
| [Skyblock Tweaks](https://modrinth.com/mod/sbt) | A Hypixel SkyBlock mod for the latest version providing many tweaks and gameplay enhancements. | [MisterCheezeCake](https://github.com/MisterCheezeCake) |
| [Firmament](https://modrinth.com/mod/firmament) | An NEU inspired Skyblock mod. | [nea890](https://github.com/nea89o) |
| [SkyCubed](https://modrinth.com/mod/skycubed) | SkyCubed is a Hypixel SkyBlock UI overhaul mod, changing all aspects of the UI in-game to be more inline into it looking like its own game. | [Meowdding](https://github.com/meowdding) |
| [Skylens](https://modrinth.com/mod/skylens) | Skylens is a highly customizable mod that shows missing enchants, has a pet overlay, a compact level display and other cool features. | [nextrg](https://github.com/nextrg) |
| [SkyOcean](https://modrinth.com/mod/skyocean) | SkyOcean is a mod that aims to improve the playing experience while staying true to the skyblock style, meaning that we aim to integrate with the base game in a seamless way. | [Meowdding](https://github.com/meowdding) |

### OptiFine Replacements

As OptiFine is no longer recommended, here are some replacements for many of it's features. Please note that some mods that have been listed in the above categories may be repeated here.

Additionally, pure performance mods are not listed here. Please check the [performance category](https://alternatives.microcontrollers.dev/latest/migrating/#performance) for those mods.

#### Features
Features that OptiFine provides that are not resource pack related.

| Mod | Description | Author | Notes |
| --- | --- | --- | --- |
| [Iris](https://irisshaders.github.io) | Shaders. More customizable than OptiFine's. | [IrisShaders](https://github.com/IrisShaders) |
| [Zoomify](https://modrinth.com/mod/zoomify) | Zoom. More customizable than OptiFine's. | [isXander](https://github.com/isXander) |
| [Cosmetica](https://modrinth.com/mod/cosmetica) (No 1.21.5 Yet) | Capes. Free, more customizable than OptiFine, and other cosmetics. | [Cosmetica-cc](https://github.com/Cosmetica-cc)
| [BetterGrassify](https://modrinth.com/mod/bettergrassify) | Better grass and snow. | [UltimatChamp](https://github.com/UltimatChamp) & [JayemCeekay](https://github.com/JayemCeekay) |
| [LambDynamicLights](https://modrinth.com/mod/lambdynamiclights) | Dynamic lights. More customizable than OptiFine. | [LambdAurora](https://github.com/LambdAurora) |
| [Fabrishot](https://modrinth.com/mod/fabrishot) (No 1.21.5 Yet) | Higher resolution Screenshots. More customizable than OptiFine. | [ramidzkh](https://github.com/ramidzkh) |

#### Resource Packs

Resource pack features that OptiFine has. Not all support the OptiFine format.

| Mod | Feature | Supports OptiFine format| Notes | Author |
| --- | --- | --- | --- | --- |
| [FabricSkyboxes](https://modrinth.com/mod/fabricskyboxes) | Custom sky. | 🚧 | Use [FabricSkyBoxes Interop](https://modrinth.com/mod/fabricskyboxes-interop) by [FlashyReese](https://github.com/FlashyReese) | [AMereBagatelle](https://modrinth.com/user/ifLBWnLs) |
| [Continuity](https://modrinth.com/mod/continuity) | Connected texture models (CTM) and emmisive textures. | ✅ | | [Pepper_Bell](https://github.com/PepperCode1) |
| [MoreMcmeta](https://modrinth.com/mod/moremcmeta) | Animated textures. | ✅ | | [soir20](https://github.com/soir20) |
| [OptiGUI](https://modrinth.com/mod/optigui) | GUI/Container textures. | ✅ | | [opekope2](https://github.com/opekope2) |
| [CIT Resewn](https://modrinth.com/mod/cit-resewn) (No 1.21.5 Yet)| Custom item textures. | ✅ | | [SHsuperCM](https://github.com/SHsuperCM) |
| [Polytone](https://modrinth.com/mod/polytone) | Custom colors, sounds, particles, GUI elements, and more. | ✅ | More customizable. | [MehVahdJukaar](https://github.com/MehVahdJukaar)  |
| [Entity Model Features](https://modrinth.com/mod/entity-model-features) | Custom entity models. | ✅ | More customizable. | [Traben](https://github.com/Traben-0) |
| [Entity Texture Features](https://modrinth.com/mod/entitytexturefeatures) | Random and emissive entity textures. | ✅ | More customizable. | [Traben](https://github.com/Traben-0) |
| [Entity Sound Features](https://modrinth.com/mod/esf) | Entity sound variation. | ✅ | More customizable. | [Traben](https://github.com/Traben-0) |
| [JsonEM](https://modrinth.com/mod/jsonem) (No 1.21.5 Yet) | Custom JSON Entity Models. | ⛔ | | [FoundationGames](https://github.com/FoundationGames) |
| [Transparent](https://modrinth.com/mod/transparent) | Transparent/translucent entities. | ✅ | | [Trikzon](https://github.com/Trikzon) |
| [Puzzle](https://modrinth.com/mod/puzzle) | Custom splash screen, better logo blending, unlimited model rotations, and bigger custom models. | ✅ | | [PuzzleMC](https://github.com/PuzzleMC) |
| [Custom Splash Screen](https://modrinth.com/mod/custom-splash-screen) (No 1.21.5 Yet) | Custom splash screen. | ⛔ | More customizable (than OptiFine and Puzzle). | [Motschen](https://github.com/Motschen) |

### Internal Shader

If you are one of those weirdos who uses internal shaders (you shouldn't btw), here's a mod that does the same thing.

| Mod | Description | Author
| --- | --- | --- |
| [Simply No Shading](https://modrinth.com/mod/simply-no-shading) | Internal Shaders. | [StartsMercury](https://github.com/StartsMercury) |

### Unrecommended Mods

These are mods that are not recommended for use. They have either been replaced by other mods, cause issues, or are simply not needed.

#### Will Never Be Supported

| Mod | Reasoning | Author |
| --- | --- | --- |
| Embeddium | Embeddium is a fork of Sodium with worse performance, worse compatability, and less features. There is no reason to use this mod. | [embeddedt](https://github.com/embeddedt) |
| More Culling | This mod is made by a user who was been exposed for making malware. Additionally, it causes many weird crashes. | [fxmorin](https://github.com/fxmorin) |
| MemoryLeakFix | This mod is made by a user who was been exposed for making malware. Additionally, this mod does next to nothing and it too causes many weird crashes. | [fxmorin](https://github.com/fxmorin) |
| ThreatenGL | This mod does not actually improve performance, as stated by both Jellysquid and IMS. It attempts to force the game to use a newer OpenGL version but does not do anything with it. | [Numelon](https://github.com/Numelon-Softworks) |
| GpuTape | This mod simply does nothing. | [ITsMrToad](https://github.com/ITsMrToad) |
| Palladium | This mod has questionable improvements and causes many crashes with other mods, including Iris. | [ITsMrToad](https://github.com/ITsMrToad) |
| Not Enough Crashes | NEC regularly causes the game to be in an invalid state and blames the wrong mods for crashes, making it harder for mod devs to debug. It is also marked incompatible with Iris and possibly other mods. | [natanfudge](https://github.com/natanfudge) |
| Better Beds | BetterBeds has been replaced by Enhanced Block Entities. Feel free to use if Enhanced Block Entities is not yet updated to the current version.| [Motschen](https://github.com/Motschen) |
| ToolTipFix | ToolTipFix has been replaced by [Adaptive Tooltips](https://modrinth.com/mod/adaptive-tooltips). | [kyrptonaught](https://github.com/kyrptonaught) |
| Animatica | Animatica has been replaced by [MoreMcMeta](https://modrinth.com/mod/moremcmeta). | [FoundationGames](https://github.com/FoundationGames) |
| Clear Void | Clear Void has been replaced by [Smooth Skies](https://modrinth.com/mod/smooth-skies). | [yezhiyi9670](https://github.com/yezhiyi9670) |
| Clear Skies | Clear Skies has been replaced by [Smooth Skies](https://modrinth.com/mod/smooth-skies). | [grondag](https://github.com/grondag) |

# Notes

Join my [Discord server](https://discord.gg/rejfv9kFJj) for news regarding the development of this repository!

If you would like to contribute, please make a PR.  
Notes:

* Leave your name and GitHub link in the contributors credits section in alphabetical order, even for a tiny change
* Please try to use Modrinth/GitHub links over CurseForge links whenever possible (Modrinth is preferred over GitHub).
* When crediting authors, please use a GitHub link instead of a Modrinth/CurseForge author page if possible.
    * Credit the GitHub organization if the GitHub profile that owns the repository is an organization profile, don't use the person credited on Modrinth/CurseForge 
* Make sure "Allow edits by maintainers" is enabled in your PRs.

## Contributors

* [Absterge](https://github.com/Absterge)
* [BobIsMyManager](https://github.com/BobIsMyManager)
* [Flopgop](https://github.com/Flopgop)
* [glai](https://github.com/glaicodes)
* [jani270](https://github.com/jani270)
* [karmette](https://github.com/karmette)
* [Kingili](https://github.com/Kingili22)
* [KTrain](https://github.com/KTrain5169)
* [moisty](https://github.com/Mqisty)
* [nacrt](https://github.com/nacrt)
* [NoPro2024](https://github.com/NoPro2024)
* [osfanbuff](https://github.com/osfanbuff63)
* [Lisena](https://github.com/Lisenaaaa)
* [Lulonaut](https://github.com/Lulonaut)
* [Mayaqq](https://github.com/MayaqqDev)
* [voxxal](https://github.com/voxxal)
* [Wyvest](https://github.com/Wyvest)
* [yedonbro](https://github.com/yedonbro)
