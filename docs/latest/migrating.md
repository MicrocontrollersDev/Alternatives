# Migrating to Latest 

This is a comprehensive guide on how to download Fabric and mods for it. It also provides direct links to many mods that you may find useful.

## Introduction

If you want more information on Fabric, why Forge/OptiFine are not recommended, or need help downloading Fabric and mods for it, click on the `Introduction` drop down below. If you are just here to see the mods list, continue to the next section.

??? note "Introduction"

    ### The Situation

    So, you've been playing 1.8.9 for the past [8 years](https://howoldisminecraft189.today) and are ready to see what 1.20.4 has to offer. Your first thought may be to download and install Forge and then add OptiFine as a mod, but this could not be further from the best choice. As Mojang has been rolling out releases, they've also been decreasing performance with every version, and neither Forge nor OptiFine are really able to bring back even a speck of that performance we see in 1.12 and below. However, another mod loader, Fabric, which is lightweight and easier to develop for, has created an amazing community in which many of its members focus on helping optimize the game to its greatest potential.

    ### Why no longer OptiFine?

    OptiFine no longer provides the benefit that it once did on older versions of the game. As the years have gone by and Minecraft's code has changed, OptiFine has been continuing to completely overwrite major parts of Minecraft's code. Because OptiFine is closed source, it has become increasingly harder for modders to provide OptiFine compatibility. OptiFine also uses outdated formats for many of its features, including MCPatcher and its confusing and outdated settings menu. Many members in the Fabric community have taken it upon themselves to create better performance enhancing mods which surpass OptiFine, as well as provide alternatives to many of OptiFine's iconic features.

    While there is a Fabric compatibility layer for OptiFine known as OptiFabric, it is unsupported by many of the mods on the list, with some outright preventing the game from loading if OptiFabric is present. Therefore, consider all mods in this list to be incompatible with OptiFabric.

    ### Why no longer Forge?

    Forge has always been less than ideal for performance due to its large overhead for server-sided modding, which is not necessary for users wishing for a vanilla compatible experience. Fabric on the other hand is extremely lightweight and is practically identical to vanilla. It's also considered to be much easier to make mods for.

    ### Installing Fabric

    Due to many issues with the official Minecraft launcher, we will not be using it. We will be using Prism Launcher instead, which is a much improved launcher that has many more features than the official Minecraft launcher and is made with mods in mind.

    First let's install the correct version of Java. In order to download Java, we will first head to the [Adoptium download page](https://adoptium.net/temurin/releases/). Adoptium is an open source Java that does not require a paid account to install, and is made by the Eclipse Foundation, a very reputable source. To install, we will use the dropdown boxes to make it easier to find the versions of Java we need

    - Operating System: (Your OS)
    - Architecture: (Your architecture, most likely x64, but check)
    - Package Type: JRE
    - Version: 17

    First install from [Prism Launcher](https://prismlauncher.org) and make sure to install the correct version. Do not download the "Portable" version unless you specifically want it. Continue the installation process until you get to the "Java" screen. Here, you will decide which Java you want to set as the default for new instances. Click on the version that says "17" at the beginning of the version and has "Eclipse Foundation" in the path name. This is your Java 19 and it will be the default version of Java for every new instance you create on Prism. Of course, you can always change this later and can still manually specify a different version of Java whenever you want.

    Now that we've installed Prism, let's log in. Once Prism has launched, you should see a Steve head and "Profiles" text in the top right. Click on this and press "Manage Accounts". From here, click "Add Microsoft" on the right side menu. This will open a popup window, which will have a button to open the link to verify yourself and also copy the code. Simply paste the code into the window that opens up. Note, you may need to sign in to your Microsoft account first.

    Once this is completed, you can exit back to the main Prism Launcher menu. Click on the button at the top left that says "Add Instance". Name it whatever you want and giving a group for it is optional, but I do not recommend giving a group name until you need to better organize your instances.

    Under the `Version` selector, find 1.20.4 and select it. Then in the `Mod Loader` tab directly underneath, choose Fabric. It will automatically choose the latest version of Fabric for 1.20.4 for you. Simply click "OK" to proceed. You should now be back on the main Prism page.

    ### Downloading and Installing Mods for Fabric

    This list currently consists of three different sources for mod downloads: Modrinth, GitHub, and CurseForge. This section will explain how to download mods from each of them.

    #### Automatic Installation:
    
    - If you are using Prism Launcher, you can simply go to the mods menu for your instance and press the "Download Mods" button in the top right to search Modrinth and CurseForge directly inside the launcher.

    - Some CurseForge mods may not allow downloads from third party launchers such as Prism Launcher. This can be bypassed by opening Prism settings, going to `APIs`, then `API Keys` and entering `$2a$10$bL4bIL5pUWqfcO7KQtnMReakwtfHbNKh6v1uTpKlzhwoueEJQnPnm` into the CurseForge Core API.

    - GitHub or non-Modrinth/CurseForge mods will require manual installation.

    #### Manual Download

    - Modrinth:
        - On the mod's page, click on the `Versions` tab. From there, you can see all versions of the mod. Make sure you download the correct one based on the Minecraft version and mod loader, click on the download icon for the newest version of the mod that fits both previous criteria.

    - GitHub:
        - For your convenience, all GitHub links lead directly to the latest version of the mod. From here, click on the `Assets` drop down if needed, then download the jar that does not include `-sources` or `-dev` in the name.
            - If a link does not redirect you to the latest version but rather the main page, on the right side of the page, you should find a tag icon with the latest version.
        - Mods downloaded this way will not automatically be installed to your instance. See the "[Manually Installing Mods on Fabric](https://alternatives.microcontrollers.dev/latest/migrating/#manually-installing-mods-on-fabric)" section on how to install these mods.

    - CurseForge:
        - Click on the `Files` tab. Look for the versions of the mod with the Minecraft version you desire and is for the Fabric mod loader, and download the latest one. You can also press the `View All` button, then sort by mod loader or Minecraft version to make finding the correct jar easier.

    #### Manually Installing Mods

    0. Close Minecraft if open.
    1. Click on your Prism Instance.
    2. Click `Edit`.
    3. Go to the `Mods` tab.
    4. Either drag and drop files into this menu, or you can press `View Folder` to drag and drop mods directly into your mods folder.
    5. You can now launch the instance.

    ### Still Need Help?

    Feel free to join my [Discord server](https://discord.gg/rejfv9kFJj) for any help downloading Fabric, its mods, or general questions about them.
    
## Mods

### Dependencies

These are essential mods that are required for some fabric mods to work.

Dependencies are going through a makeover where along with a giant list at the top, mods will specify their required dependencies in the table itself. This is currently only implemented for a few categories.

| Mod | Required for | Author |
| --- | --- | --- |
| [Fabric API](https://modrinth.com/mod/fabric-api) | Most mods | [Fabric Team](https://github.com/FabricMC) |
| [Fabric Language Kotlin](https://modrinth.com/mod/fabric-language-kotlin) | Several mods (that use kotlin) | [Fabric Team](https://github.com/FabricMC) |
| [Mod Menu](https://modrinth.com/mod/modmenu) | Most mods | [Terraformers](https://github.com/TerraformersMC) |
| [Indium](https://modrinth.com/mod/indium) | Several mods | [comp500](https://github.com/comp500) |
| [Architectury](https://modrinth.com/mod/architectury-api) | Several mods | [Shedaniel](https://github.com/shedaniel) |
| [Cloth Config](https://modrinth.com/mod/cloth-config) | Several mods | [Shedaniel](https://github.com/shedaniel) |
| [YetAnotherConfigLib](https://modrinth.com/mod/yacl) | Several mods | [isXander](https://github.com/isXander)
| [MaLiLib](https://www.curseforge.com/minecraft/mc-mods/malilib) | Litematica, MiniHUD | [Matti Ruohonen](https://github.com/maruohon) |
| [Ash API](https://modrinth.com/mod/ash-api) | Transparent. | [Trikzon](https://github.com/Trikzon) |
| [Searchables](https://modrinth.com/mod/searchables) | Controlling | [Jaredllll08](https://github.com/jaredlll08) |
| [DarkKore](https://modrinth.com/mod/darkkore) (No 1.20.4 Yet) | KronHUD | [DarkKronicle](https://github.com/DarkKronicle) |
| [Lilac](https://modrinth.com/mod/lilac) | OptiGUI | [opekope2](https://github.com/opekope2) |

### Performance

These are mods that are needed for playing the latest versions of Minecraft at a reasonable FPS. These will also help decrease frame times, hopefully eliminating spikes or stuttering.

| Mod | Description | Author | Dependencies | Incompatabilities | Notes |
| --- | --- | --- | --- | --- | --- |
| [Sodium](https://modrinth.com/mod/sodium) | An all around performance mod, Sodium allows users to play the latest versions of Minecraft with high FPS, completely outperforming OptiFine, with some users seeing up to 8x their vanilla frames. Sodium also drastically improve visuals, providing a much better gameplay experience. | [CaffeineMC](https://github.com/CaffeineMC) |
| [Iris](https://modrinth.com/mod/iris) | A shader loader that allows users to load up their favorite OptiFine shaderpacks, but with much higher FPS. Iris also provides performance enhancements when not using shaders, making it great for all users. | [Iris Team](https://github.com/IrisShaders) | [Sodium](https://modrinth.com/mod/sodium) |
| [Lithium](https://modrinth.com/mod/lithium) | Helps improve the performance of many vanilla systems without changing their mechanics. | [CaffeineMC](https://github.com/CaffeineMC) |
| [Exordium](https://modrinth.com/mod/exordium) | Caps the FPS of certain HUD elements that do not need to be updated every frame. | [tr7zw](https://github.com/tr7zw) | [Fabric API](https://modrinth.com/mod/fabric-api) | | May break some HUD elements from other mods. |
| [DashLoader](https://modrinth.com/mod/dashloader) (No 1.20.4 Yet) | Caches all of Minecraft's contents to load the game much faster and provide insanely quick reloads. | [alphaqu](https://github.com/alphaqu) |
| [Enhanced Block Entities](https://modrinth.com/mod/ebe) (No 1.20.4 Yet) | Improves block entities by making them used baked models instead, allowing for better performance, visuals (via better smoothlighting), and better resource pack customizability. | [FoundationGames](https://github.com/FoundationGames) | [Fabric API](https://modrinth.com/mod/fabric-api) |
| [FerriteCore](https://modrinth.com/mod/ferrite-core) | Helps reduce the amount of memory the game takes up. This may make a big difference for larger modpacks as well. | [malte0811](https://github.com/malte0811) |
| [Entity Culling](https://modrinth.com/mod/entityculling) | Culls entities that you cannot see, increasing FPS. While Sodium already does this, this mod is much more thorough in which entities can be culled. | [tr7zw](https://github.com/tr7zw) |
| [More Culling](https://modrinth.com/mod/moreculling) | Culls more block faces not already culled by Sodium. Can provide a massive performance boost when many of these blocks are in view. | [fxmorin](https://github.com/fxmorin) | [Cloth Config](https://modrinth.com/mod/cloth-config) |
| [ImmediatelyFast](https://modrinth.com/mod/immediatelyfast) | Improves the immediate mode rendering performance. | [RaphiMC](https://github.com/RaphiMC) |
| [Dynamic FPS](https://modrinth.com/mod/dynamic-fps) | Reduces your FPS when tabbed out of the game, therefore reducing your system load. | [juliand665](https://github.com/juliand665) | [Fabric API](https://modrinth.com/mod/fabric-api) |
| [Lazy Language Loader](https://modrinth.com/mod/lazy-language-loader) | Improves loading times when changing your language in game by only reloading the required resources. | [chachy](https://github.com/ChachyDev) |
| [Sodium Extra](https://modrinth.com/mod/sodium-extra) | Allows you to half the resolution on Apple's Retina displays and also adds most of OptiFine's performance features such as toggles for animations, particles, rain/snow, clouds, sky and biome colors, and more, as well as some custom ones. | [FlashyReese](https://github.com/FlashyReese) | [Fabric API](https://modrinth.com/mod/fabric-api), [Sodium](https://modrinth.com/mod/sodium) |
| [Debugify](https://modrinth.com/mod/debugify) | Fixes several bugs in Minecraft, including a few which can effect performance. This will fix lag spikes when crossing chunks and when clicking on links or the resource pack folder button, reduces time it takes to load into a world, and fixes entity collision checks being needlessly calculated client side. | [isXander](https://github.com/isXander) | [YACL](https://modrinth.com/mod/yacl) |
| [Audio Engine Tweaks](https://modrinth.com/mod/audio-engine-tweaks) (No 1.20.4 Yet) | Fixes the sound pool overloading, allowing for sounds to continue playing at all time and without log spam. | [mattymatty97](https://github.com/mattymatty97) |
| [FastAnim](https://modrinth.com/mod/fastanim) (No 1.20.4 Yet) | Speeds up entity angle calculations, which may be especially noticeable when there is a high number of entities on screen. | [Lunade_](https://github.com/AViewFromTheTop) |
| [Ksyxis](https://modrinth.com/mod/ksyxis) | Reduces world loading times. | [VidTu](https://github.com/VidTu) |
| [FastQuit](https://modrinth.com/mod/fastquit) | Allows you to go back to the title screen while the world is still loading or saving. It is done in a way that prevents world corruption. | [KingContaria](https://github.com/KingContaria) | [Fabric API](https://modrinth.com/mod/fabric-api), [Cloth Config](https://modrinth.com/mod/cloth-config) |
| [Noxesium](https://modrinth.com/mod/noxesium) | Contains several smaller performance improvements and also has many visual bug fixes for the MCCI server. | [Noxcrew](https://github.com/Noxcrew) | [Fabric API](https://modrinth.com/mod/fabric-api) |
| [Remove Reloading Screen](https://modrinth.com/mod/rrls) | Allows you to access other parts of the game by removing the reload screen except for the progress bar. | [dima_dencep](https://github.com/dimadencep) | [Fabric API](https://modrinth.com/mod/fabric-api), [Cloth Config](https://modrinth.com/mod/cloth-config) |
| [C2ME](https://modrinth.com/mod/c2me-fabric) | C2ME is an experimental mod that attempts to multithread chunk generation, I/O, and loading. | [RelativityMC](https://github.com/RelativityMC) |
| [Very Many Players](https://modrinth.com/mod/vmp-fabric) | VMP attempts to alleviate the strain on servers when there are a large amount of players. | [RelativityMC](https://github.com/RelativityMC) |
| [Early Loading Screen](https://modrinth.com/mod/early-loading-screen) | Allows the game to create a game window earlier, allowing you to stop the game much faster if needed. | [Ishland](https://github.com/ishland) | | | May cause crashes when starting the game. If your game instantly crashes, try disabling this mod. |
| [Noisium](https://modrinth.com/mod/noisium) | Optimizes world generation when generating new chunks. | [Steveplays](https://github.com/Steveplays28) |

### Other Performance Mods

These are other performance mods that one may prefer to use, but are not required. It is neither recommended or unrecommended, and is up to the player to decide given their use-case.

| Mod | Description | Author | Dependencies | Incompatabilities | Notes |
| --- | --- | --- | --- | --- | --- |
| [Nvidium](https://modrinth.com/mod/nvidium) | Nvidium uses NVIDIA only OpenGL extensions to greatly improve the game's performance. This mod will not work on AMD. It has a few graphical glitches and could lead to crashes, as the mod is still in beta and not considered stable yet. The mod will also disable itself whenever Iris shaders are enabled or if the required OpenGL extensions are not available. | [MCRcortex](https://github.com/MCRcortex) | [Sodium](https://modrinth.com/mod/sodium) | | Chunks won't fade when using [Chunks Fade In](https://modrinth.com/mod/chunks-fade-in). |
| [Fadeless](https://modrinth.com/mod/fadeless) | Removes transitions such as the fading animation that Mojang added between their splash screens. This may provide a smoother experience if the fade is choppy on a low end machine or allow people to access certain menus quicker if they do not like the small wait time. This mod is made partially redundant by Remove Loading Screen. | [DerpDerpling](https://github.com/DerpDerpling) & [UltimateBoomer](https://github.com/UltimateBoomer) | [Fabric API](https://modrinth.com/mod/fabric-api) |
| [Krypton](https://modrinth.com/mod/krypton) | This mod is bannable on Hypixel and most likely other servers. Although it is probably not detectable, it is still against Hypixel's rules and the mod developer does not recommend using it on Hypixel. However, this mod works great for private servers. Krypton optimizes network stacking and entity tracking, as well as other micro-optimizations. | [astei](https://github.com/astei) |
| [Methane](https://modrinth.com/mod/methane) | Completely kills the light engine, providing permanent fullbright and improved FPS. Disable when using shaders. Allows you to disable some fog such as powdered snow fog and lava fog, which may be considered as an unfair advantage on some servers. | [AnOpenSauceDev](https://github.com/AnOpenSauceDev) | [Fabric API](https://modrinth.com/mod/fabric-api), [Cloth Config](https://modrinth.com/mod/cloth-config) | | May cause issues when using some shaders. Disable Methane if there are visual glitches. |
| [Sciophobia](https://modrinth.com/mod/sciophobia) | Removes text shadows globally. Due to Minecraft's not so great text rendering, this can greatly improve performance, especially when a lot of text is being rendered on the screen at once, with the trade-off that text looks terrible and can sometimes be near impossible to read. May help on especially terrible computers, but for most people this is more of a preference thing than a performance improvement. | [MicrocontrollersDev](https://github.com/MicrocontrollersDev) | [Fabric API](https://modrinth.com/mod/fabric-api), [YACL](https://modrinth.com/mod/yacl) |

### Recommended

These are mods that I personally recommend due to their usefulness. While they may not boost performance, they are mostly quality of life mods meant to better your experience.

| Mod | Description | Author | Notes |
| --- | --- | --- | --- |
| [No Chat Reports](https://modrinth.com/mod/no-chat-reports) | Removes cryptographic signatures from chat messages, making it harder to get chat reported. | [Aizistral](https://github.com/Aizistral-Studios) |
| [Modern Keybinding](https://modrinth.com/mod/modernkeybinding) | Allows you to use modifiers for keybinds. For example, you can set keybinds to Ctrl/Shift/Alt + key. | [Nova-Committee](https://github.com/Nova-Committee) |
| [Model Gap Fix](https://modrinth.com/mod/modelfix) | Fixes the gaps you see on items when holding them as well as 3D blocks. This makes for a much more pleasant experience for most resourcepacks, including both defaults. | [MehVahdJukaar](https://github.com/MehVahdJukaar) | The mod author has not updated the supported Minecraft versions on the Modrinth page, but it should work with no issues regardless. |
| [Borderless Mining](https://modrinth.com/mod/borderless-mining) | Borderless Fullscreen for Minecraft. This makes the game not minimize when you tab out. | [comp500](https://github.com/comp500) | The mod author has not updated the supported Minecraft versions on the Modrinth page, but it should work with no issues regardless. |
| [Recursive Resources](https://modrinth.com/mod/recursiveresources) | Resource Pack Organizer but ported to Fabric and with more features. It allows you to sort resource packs into folders, as well as search for them using a search bar. It also lets you change how resourcepacks are ordered.
| [Smooth Scrolling Refurbished](https://modrinth.com/mod/smooth-scrolling-refurbished) | Makes the scrolling in all menus smoother. | [JustAlittleWolf](https://github.com/JustAlittleWolf) |
| [Controlling](https://modrinth.com/mod/controlling) | Completely revamps Minecraft's controls menu, making it much easier to navigate and change keys, letting you search and more easily find conflicting keybinds. | [Jaredllll08](https://github.com/jaredlll08) |
| [Better Recipe Book](https://www.modrinth.com/mod/brb) | Brings many QOL improvements to the current recipe book, making it much more useful for different scenarios. | [marshmallow](https://github.com/mrshmllow) |
| [Chat Patches](https://modrinth.com/mod/chatpatches) | Adds several QOL features to Minecraft's chat to make it more usable. | [mrbuilder1961](https://github.com/mrbuilder1961) |
| [MixinTrace](https://modrinth.com/mod/mixintrace) | Makes it easier for mod developers to debug crash reports. | [comp500](https://github.com/comp500) |
| [Adaptive Tooltips](https://modrinth.com/mod/adaptive-tooltips) (No 1.20.4 Yet) | Makes tooltips more readable by preventing them from going off screen and allowing for tooltip scrolling, as well as more customization options such as custom transparency. | [isXander](https://github.com/isXander) |
| [Persistent Stuff](https://modrinth.com/mod/persistent-stuff) (No 1.20.4 Yet) | Saves your toggle sprint (sprinting/walking), hitboxes' (enabled/disabled), chunk borders' (enabled/disabled) states across Minecraft restarts. Never toggle these at startup again. | [Andy Russo](https://github.com/AndyRusso) |
| [Log Cleaner](https://modrinth.com/mod/log-cleaner) | Automatically deletes old logs to clear up storage space. | [Altrisi](https://github.com/altrisi) | (Probably) works on 1.20.4 despite not being updated to it. |
| [Better Selection](https://modrinth.com/mod/better-selection) | Makes it easier to select text by allowing mouse selection and Ctrl + ← and Ctrl + →. | [MDLC01](https://github.com/MDLC01) |
| [AuthMe](https://modrinth.com/mod/auth-me) | Let's you easily reauthenticate when you are not logged in correctly. Can also be used to switch accounts. | [axieum](https://github.com/axieum) |

### Other Cool Mods

These are mods that are more dependant on personal preference than importance.

| Mod | Description | Author | Notes |
| --- | --- | --- | --- |
| [e4mc](https://modrinth.com/mod/e4mc) (No 1.20.4 Yet) | Let's you invite people to your singleplayer worlds! They do not need to have the mod installed for it to work. | [vgskye](https://git.skye.vg/me) |
| [Cosmetica](https://modrinth.com/mod/cosmetica) | Adds cosmetics to your game completely for free! Also supports showing cosmetics from other clients and mods! | [Cosmetica-cc](https://github.com/Cosmetica-cc) |
| [3D Skin Layers](https://modrinth.com/mod/3dskinlayers) | Makes the outer layer of skins 3D. Very customizable and lets you adjust distance that 3D renders for performance. | [tr7zw](https://github.com/tr7zw) |
| [SuperBetterGrass](https://www.curseforge.com/minecraft/mc-mods/super-better-grass) | Better grass and snow, more customizable than OptiFine. | [LambdAurora](https://github.com/LambdAurora) & [Dima-Dencep](https://github.com/dima-dencep) | This is a fork of LambdaBetterGrass by LambdAurora |
| [Overlay Tweaks](https://modrinth.com/mod/overlaytweaks) | A small QOL mod that lets you alter vanilla's overlays in small ways. | [MicrocontrollersDev](https://github.com/MicrocontrollersDev) |
| [Nametag Tweaks](https://modrinth.com/mod/nametagtweaks) | Let's you alter the way nametags are rendered, such as background transparency, text shadow, and custom F1 rules. | [MicrocontrollersDev](https://github.com/MicrocontrollersDev) |
| [Chunks Fade In](https://modrinth.com/mod/chunks-fade-in) | Adds a fade-in animation to chunks similar to Bedrock Edition. | [kerudion](https://github.com/kerudion) | Nvidium (chunks don't fade) |
| [Distant Horizons](https://modrinth.com/mod/distanthorizons) (No 1.20.4 Yet) | Adds LODs to Minecraft, allowing for much further render distances without a big tank on performance. | [James Seibel](https://gitlab.com/jeseibel) | Many shaders may cause LODs to not load or be black. |
| [Controlify](https://modrinth.com/mod/controlify) | Allows you to easily play Minecraft with a controller. | [isXander](https://github.com/isXander) |
| [CleanView](https://www.curseforge.com/minecraft/mc-mods/cleanview-fabric) | Prevents self particles from appearing on your screen. | [LianMI](https://github.com/zlainsama) |
| [Color Me Outlines](https://modrinth.com/mod/color-me-outlines) (No 1.20.4 Yet) | Color Me Outlines is a close equivalent to 1.8's block overlay, allowing you to customize the outline when looking at blocks. | [LordDeatHunter](https://github.com/LordDeatHunter) |
| [Pretty Hitboxes](https://github.com/yojan69/PrettyHitboxes-1.20.4/releases/latest) | Allows you to customize hitboxes, similar to 1.8 mods and clients. | [ErrorGamer2000](https://github.com/nexensys) & [yojan69](https://github.com/yojan69) | This is an updated fork for 1.20.4. |
| [Blur](https://modrinth.com/mod/blur-fabric) | Creates a nice blur effect when in menus and is completely customizable. | [Motschen](https://github.com/Motschen) |
| [WaveyCapes](https://modrinth.com/mod/wavey-capes) | Breaks your cape into smaller sections to make its movement more fluid. Looks great with the new migration capes. | [tr7zw](https://github.com/tr7zw) |
| [Perspektive](https://modrinth.com/mod/perspektive) **(BANNABLE ON HYPIXEL)** | A simple 360 degrees perspective mod that lets you move the camera without moving your player's direction. | [r0yzer](https://github.com/r0yzer) |
| [KronHUD](https://modrinth.com/mod/kronhud) (No 1.20.4 Yet) | Adds many useful HUD elements to your screen with an easy to use in game config. | [DarkKronicle](https://github.com/DarkKronicle) |
| [BetterF3](https://modrinth.com/mod/betterf3) | Replaces Minecraft's original debug HUD with a highly customizable, more human-readable HUD. You can customize colors, position, add spacings, and more. | [cominixo](https://github.com/cominixo) |
| [TNTTime](https://modrinth.com/mod/tnttime) | Displays time left to the TNT explosion above primed TNT. | [Simon](https://github.com/shateq) |
| [Paginated Advancements & Custom Frames](https://modrinth.com/mod/paginatedadvancements) | Makes the advancement menu fit your entire screen, which could make it easier to navigate the menu. | [DaFuqs](https://github.com/DaFuqs)
| [AppleSkin](https://modrinth.com/mod/appleskin) | Lets you know how much a food will restore your hunger bar. | [Ryan Liptak](https://github.com/squeek502) |
| [Horse Stats Vanilla](https://modrinth.com/mod/horsestatsvanilla) (No 1.20.4 Yet) | Adds the stats of your horse in your horse/donkey inventory HUD, making it easy to see the perks of your horses and donkeys. | [d4m0n](https://github.com/d4rkm0nkey) |
| [Better Mount HUD](https://modrinth.com/mod/better-mount-hud) | Makes some important HUD modules visible when riding a mount. | [Lortseam](https://github.com/Lortseam) |
| [Clear Despawn](https://modrinth.com/mod/cleardespawn) | Clear Despawn makes it more obvious on which items are about to despawn by making them blink exponentially faster after a certain time. | [StrikerRockers](https://github.com/StrikerRockers-Mods) |
| [Litematica](https://www.curseforge.com/minecraft/mc-mods/litematica) | A schematic mod that allows you to import schematics of builds. | [Matti Ruohonen](https://github.com/maruohon) |
| [MiniHUD](https://www.curseforge.com/minecraft/mc-mods/minihud) | A customizable HUD that allows displaying various information on your screen as well as beneficial overlay renders. | [Matti Ruohonen](https://github.com/maruohon) |
| [Clear Skies](https://modrinth.com/mod/clear-skies) | Removes fog color banding on skybox. | [grondag](https://github.com/grondag) | The 1.19 version works on 1.20.4. |
| [Extended Clouds](https://modrinth.com/mod/extended-clouds) (No 1.20.4 Yet) | Changes cloud render distance to be same as your set render distance. | [alphaqu](https://github.com/alphaqu) |
| [Sound Physics Remastered](https://modrinth.com/mod/sound-physics-remastered) | Makes sounds much more realistic, adding reverb, attenuation, and absorption. | [vlad2305m](https://github.com/vlad2305m), [thedocruby](https://github.com/thedocruby) & [henkelmax](https://github.com/henkelmax)|
| [Screencapper](https://modrinth.com/mod/screencapper) (No 1.20.4 Yet) | Improves the way you share and view screenshots. | [Deftu](https://github.com/Deftu) |
| [Better TaskBar](https://modrinth.com/mod/better-taskbar) (**Windows Only**) | Small mod that applies the windows progress animation to the Minecraft icon in the taskbar whenever loading resources or a world. | [MORIMORI0317](https://github.com/MORIMORI0317) |
| [Better Command Block UI](https://modrinth.com/mod/bettercommandblockui) | Improves the command block user interface by allowing for visual newlining . | [Tectato](https://github.com/Tectato) |
| [Better Statistics Screen](https://modrinth.com/mod/better-stats) | A visual overhaul to the statistics screen, giving useful information in a much more visually appealing format. | [TheCSDev](https://github.com/TheCSDev) |
| [Chat Heads](https://modrinth.com/mod/chat-heads) | Shows a player's head next to their chat message in game. | [dzwdz](https://github.com/dzwdz) |
| [ChatShot](https://modrinth.com/mod/chatshot) | Allow easy screenshotting of chat messages. | [DeDiamondPro](https://github.com/DeDiamondPro) |
| [Craftify](https://modrinth.com/mod/craftify) | Shows your currently playing music on your HUD. | [ThatGravyBoat](https://github.com/ThatGravyBoat) |
| [Reimagined World Menu](https://modrinth.com/mod/reimagined-world-menu) | Redesigns the world creation screen. | [Iamaprogramer](https://github.com/lamaprogramer) |
| [Resourcify](https://modrinth.com/mod/resourcify) | Lets you view, download, and update resource packs from Modrinth all in game. | [DeDiamondPro](https://github.com/DeDiamondPro) |
| [Make Bubbles Pop](https://modrinth.com/mod/make_bubbles_pop) | Improves the look of bubbles in water. | [Tschipcraft](https://github.com/Tschipcraft) |
| [NoRefreshScroll](https://modrinth.com/mod/norefreshscroll) | Stops the multiplayer screen from scrolling to bottom when refreshing. | [Thatsmusic99](https://github.com/Thatsmusic99) |
| [Particle Tweaks](https://modrinth.com/mod/particle-tweaks) | Makes particles look nicerby adding growing/fading effects and water physics. | [Lunade_](https://github.com/AViewFromTheTop) |
| [Particle Rain](https://modrinth.com/mod/particle-rain) | Replaces the rain effect with particles. | [PigCart](https://github.com/PigCart) |
| [SkinShuffle](https://modrinth.com/mod/skinshuffle) | Allows you to change, store, and customize your skins in game. | [mineblock11](https://github.com/mineblock11) |
| [Tiny Item Animations](https://modrinth.com/mod/tiny-item-animations) | Adds a small animation when holding items similar to old console editions of the game. | [Trivaxy](https://github.com/Trivaxy) |
| [Draggable Lists](https://modrinth.com/mod/draggable-lists) | Allows you to drag to order resourcepacks, datapacks, worlds, and servers. | [MrMelon54](https://github.com/MrMelon54) |
| [Highlight](https://modrinth.com/mod/highlight) (No 1.20.4 Yet) | Changes hitboxes to allow them to not be axis alligned, making them look much smoother on some blocks. | [Team Resourceful](https://github.com/Team-Resourceful) |
| [Biome Moss](https://modrinth.com/mod/biome-moss) (No 1.20.4 Yet) | Improves the look of moss by adding color biome variation. | [TheDarkCoder](https://github.com/TheDarkCoder) |
| [Fluid Void Fading](https://modrinth.com/mod/fluidvoidfading) (No 1.20.4 Yet) | Makes liquids like water and lava slowly fade out in the void. Looks great in games like Skyblock, Skyways, or similar. | [DaFuqs](https://github.com/DaFuqs) |
| [Server Pinger Fixer](https://modrinth.com/mod/serverpingerfixer) | Makes server pinging smoother and fixes it breaking when refreshing too many times. | [JustAlittleWolf](https://github.com/JustAlittleWolf) |
| [Axiom](https://modrinth.com/mod/axiom) | An alternative to WorldEdit and VoxelSniper to make building in singleplayer much easier. | [Moulberry](https://github.com/Moulberry) |
| [Sounds](https://modrinth.com/mod/sound) | Adds many more sounds to Minecraft for things that did not previously have sounds. | [mineblock11](https://github.com/mineblock11) |

### OptiFine Replacements

As OptiFine is no longer recommended, here are some replacements for many of it's features. Please note that some mods that have been listed in the above categories may be repeated here.

#### Features
Features that OptiFine provides that are not resource pack related.

| Mod | Description | Author | Notes |
| --- | --- | --- | --- |
| [Iris](https://irisshaders.github.io) | Shaders. More customizable than OptiFine's. | [IrisShaders](https://github.com/IrisShaders) |
| [Zoomify](https://modrinth.com/mod/zoomify) | Zoom. More customizable than OptiFine's. | [isXander](https://github.com/isXander) |
| [Cosmetica](https://modrinth.com/mod/cosmetica) | Capes. Free, more customizable than OptiFine, and other cosmetics. | [Cosmetica-cc](https://github.com/Cosmetica-cc)
| [SuperBetterGrass](https://www.curseforge.com/minecraft/mc-mods/super-better-grass) | Better grass and snow, more customizable than OptiFine. | [LambdAurora](https://github.com/LambdAurora) & [Dima-Dencep](https://github.com/dima-dencep) | This is a fork of LambdaBetterGrass by LambdAurora. |
| [LambDynamicLights](https://modrinth.com/mod/lambdynamiclights) | Dynamic lights. More customizable than OptiFine. | [LambdAurora](https://github.com/LambdAurora) |
| [Fabrishot](https://modrinth.com/mod/fabrishot) | Higher resolution Screenshots. More customizable than OptiFine. | [ramidzkh](https://github.com/ramidzkh) |

#### Resource Packs

Resource pack features that OptiFine has. Not all support the OptiFine format.

| Mod | Feature | Supports OptiFine format| Notes | Author |
| --- | --- | --- | --- | --- |
| [FabricSkyboxes](https://modrinth.com/mod/fabricskyboxes) | Custom sky. | 🚧 | Use [FabricSkyBoxes Interop](https://modrinth.com/mod/fabricskyboxes-interop) by [FlashyReese](https://github.com/FlashyReese) | [AMereBagatelle](https://modrinth.com/user/ifLBWnLs) |
| [Continuity](https://modrinth.com/mod/continuity) | Connected texture models (CTM) and emmisive textures. | ✅ | | [Pepper_Bell](https://github.com/PepperCode1) |
| [MoreMcmeta](https://modrinth.com/mod/moremcmeta) | Animated textures. | ✅ | | [soir20](https://github.com/soir20) |
| [OptiGUI](https://modrinth.com/mod/optigui) | GUI/Container textures. | ✅ | | [opekope2](https://github.com/opekope2) |
| [Translucency Fix](https://modrinth.com/mod/translucencyfix) | Fixes semitranslucent textures. | 🚧 | Not sure if OptiFine even does this. | [ruvaldk](https://github.com/ruvaldak) |
| [CIT Resewn](https://github.com/dicedpixels/CITResewn/releases/latest) | Custom item textures. | ✅ | This is a 1.20.4 updated fork by [dicedpixels](https://github.com/dicedpixels). | [SHsuperCM](https://github.com/SHsuperCM) |
| [Vanadium](https://modrinth.com/mod/vanadium) (No 1.20.4 Yet) | Custom colors. | ✅ | | [AlucardMG36](https://github.com/AlucardMG36) |
| [Entity Model Features](https://modrinth.com/mod/entity-model-features) | Custom entity models. | ✅ | More customizable. | [Traben](https://github.com/btrab1) |
| [Entity Texture Features](https://modrinth.com/mod/entitytexturefeatures) | Random and emissive entity textures.| ✅ | More customizable. | [Traben](https://github.com/btrab1) |
| [JsonEM](https://modrinth.com/mod/jsonem) (No 1.20.4 Yet) | Custom JSON Entity Models. | ⛔ | | [FoundationGames](https://github.com/FoundationGames) |
| [Transparent](https://modrinth.com/mod/transparent) | Transparent/translucent entities. | ✅ | | [Trikzon](https://github.com/Trikzon) |
| [Puzzle](https://modrinth.com/mod/puzzle) | Custom splash screen, better logo blending, unlimited model rotations, and bigger custom models. | ✅ | | [PuzzleMC](https://github.com/PuzzleMC) |
| [Custom Splash Screen](https://modrinth.com/mod/custom-splash-screen) (No 1.20.4 Yet) | Custom splash screen. | ⛔ | More customizable (than OptiFine and Puzzle). | [Motschen](https://github.com/Motschen) |

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
| MemoryLeakFix | While this mod does fix some memory leaks, it's rendered almost entirely useless when using FerriteCore and may causes issues and crashes with other mods, and the leaks it fixes are not major enough to be worth it. | [fxmorin](https://github.com/fxmorin) |
| Starlight | Starlight rewrotes the light engine to make loading chunks much quicker. Mojang has now included this fix in 1.20 and Starlight is no longer needed. Despite the fact that updates are still being made, the developer says there is no point in using them. | [Spottedleaf](https://github.com/Spottedleaf) |
| Not Enough Crashes | NEC regularly causes the game to be in an invalid state and blames the wrong mods for crashes, making it harder for mod devs to debug. It is also marked incompatible with Iris and possibly other mods. | [natanfudge](https://github.com/natanfudge) |
| Better Beds | BetterBeds has been replaced by Enhanced Block Entities. Feel free to use if Enhanced Block Entities is not yet updated to the current version.| [Motschen](https://github.com/Motschen) |
| ToolTipFix | ToolTipFix has been replaced by Adaptive Tooltips. | [kyrptonaught](https://github.com/kyrptonaught) |
| Animatica | Animatica has been replaced by MoreMcMeta. | [FoundationGames](https://github.com/FoundationGames) |

# Notes

Join my [Discord server](https://discord.gg/rejfv9kFJj) for news regarding the development of this repository!

If you would like to contribute, please make a PR.  
Some notes:
- Leave your name and GitHub link in the contributors credits section in alphabetical order, even for a tiny change
- Please try to use Modrinth or GitHub over CurseForge when possible (Modrinth is the preferred platform)
- Please use a GitHub link instead of a Modrinth/CurseForge link for Author credit when possible
    - If the GitHub profile is an organization, use that instead of one of the owners / person credited on Modrinth/CurseForge
- Make sure that the option to allow me to make changes to your PR is enabled

## Contributors

* [Absterge](https://github.com/Absterge)
* [BobIsMyManager](https://github.com/BobIsMyManager)
* [Flopgop](https://github.com/Flopgop)
* [glai](https://github.com/glaicodes)
* [karmette](https://github.com/karmette)
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
