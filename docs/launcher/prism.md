# Prism Launcher

Prism Launcher is an incredibly powerful launcher that makes managing your mods and modded instances much easier. It can do everything the official launcher can do, but allows for much more customization and ease of access. The official launcher is much slower to use and requires a lot of manual work for modern Minecraft. For modded and vanilla users alike, it is recommended to switch to Prism Launcher for an issue-less experience.

This guide will explain the install process for Prism. Please take the time after setting up to better learn your way around the launcher, as you may end up using it as your go-to launcher from now on!

## How to Install

* Despite looking long, this is a very simple process and should only take a few minutes!

### Step 1 - Installing Prism

[Download Prism Launcher](https://prismlauncher.org/download). Download the correct version your system and begin the installation. For Linux users, install through your package manager (Flathub or distro if available).

For the Minimum and Maximum memory allocation, leave them at 512 MiB and 4096 MiB respectively, unless you only have 8GB of ram or less, in which case you may want to change the maximum to 2048 MiB.

All of these settings can be later adjusted globally or per instance. This includes changing the Java version or memory allocation. See the global settings button on the main page or in instance settings once you've completed this guide.

After this, continue with the installation process as normal.

### Step 2 - Logging in

Now that we've installed Prism, let's log in. Once Prism has launched, you should see a Steve head and `Profiles` text in the top right. Click on this and press "Manage Accounts". From here, click `Add Microsoft` on the right side menu. This will open a popup window, which will have a button to open the link to verify yourself and also copy the code. Simply paste the code into the window that opens up. Note, you may need to sign in to your Microsoft account first.

Once this is completed, you can exit back to the main Prism Launcher menu. Click on the button at the top left that says "Add Instance".

### Step 3 - Creating an instance

This guide will describe the process for Fabric 1.21.10, but steps for other versions should also be obvious.

Once you've clicked on the button on the top left that says `Add Instance`, name it whatever you want and giving a group for it is optional, but I do not recommend giving a group name until you need to better organize your instances.

Under the `Version` selector, select 1.21.10. Then in the `Mod Loader` tab directly underneath, choose Fabric. It will automatically choose the latest version of Fabric for 1.21.10 for you. Simply click "OK" to proceed. You should now be back on the main Prism page.

### Step 4 - Installing Mods

You can manage all your mods by clicking on the instance and pressing `Edit`, then clicking the `Mods` tab.

If the mod is on Modrinth or CurseForge, download them within the launcher using the `Download Mods` button. You should prioritize checking Modrinth first (the default selection in Prism). If the mod is not on either, you should be confident that it is not malware/a RAT, and you can simply drag and drop them into the Mods tab in Prism. 

You can similarly install resource and shader packs in their own tabs.

## Updating Prism, Mods, Minecraft, and Fabric Loader

**To update Prism**, an update button will appear on the top toolbar when an update is available.

**To update mods**, head to the `Mods` tab, and simply press the `Check for Updates` button and follow all prompts. This will update all your mods to the latest version. It can also update disabled mods, but will still keep them disabled by default.

**To update Minecraft**, head to the `Version` tab, (right) click on `Minecraft`, then `Change Version`. Set it to the version you want to use. Update your mods as described in the step above to update your mods to the new Minecraft version as well. Not all mods may be available for this new version of Minecraft. Take note of which mods don't get updated and try playing. If you crash, read the crash message to see which mods aren't updated yet and disable them.

**To update Fabric Loader**, head to the `Version` tab, (right) click on `Fabric Loader`, then `Change Version`. Set it to the latest version.

## CurseForge API Key

Some CurseForge mods may not allow downloads from third party launchers such as Prism Launcher. This can be bypassed by opening Prism settings, going to `Services`, then `API Keys` and entering `$2a$10$bL4bIL5pUWqfcO7KQtnMReakwtfHbNKh6v1uTpKlzhwoueEJQnPnm` into the CurseForge text box.

## Themes

You can find a list of Prism themes and how to install them on [their website](https://prismlauncher.org/wiki/getting-started/change-themes).

## Common Issues

#### `My mods aren't showing up in-game!`

If you see a list of mods in the `Mods` tab, you should click `Version` and check if `Fabric Loader` is installed. If not, press `Install Loader` on the right and install the latest version of Fabric Loader.

<br>

## Need More Help?

If you encounter any issues not shown here you should ask for help in my [discord server](https://discord.gg/rejfv9kFJj).
If you encounter any issues **unrelated to the guide at all**, or if you want to be in their community or follow for updates, you can ask in the [Prism Community discord server](https://discord.gg/prism-community-1031648380885147709)

# Contributors

* [KTrain](https://github.com/KTrain5169)
* [ooTruffle](https://github.com/ooTruffle)
* [PandaNinjas](https://github.com/pandaninjas)
* [Shiggy](https://github.com/Shiggy-dev)
