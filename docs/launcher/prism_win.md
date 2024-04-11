# Prism Launcher

Prism Launcher is an incredibly powerful launcher that makes managing your mods and modded instances much easier. It can do everything the official launcher can do, but allows for much more customization and ease of access. The official launcher has had several issues that have taken weeks to fix or are currently still not fixed, despite their severity. For modded and vanilla users alike, it is recommended to switch to Prism Launcher for an issue-less experience.

This guide will explain the install process for Prism, as well as how we can use it for SkyClient. Please take the time after setting up to better learn your way around the launcher, as you may end up using it as your go-to launcher from now on!

## How to Install (Windows)

- Despite looking long, this is a very simple process and should only take a few minutes! This guide will also assume you are migrating from SkyClient, but steps will be largely the same, except for the migrating data section.

### Step 1 - Installing Java

First, we need to download and setup Java to be able to use Prism Launcher. Unlike the default Minecraft launcher, Prism does not come bundled with a default Java, and so we must install it ourselves.

Minecraft 1.16 and below all use Java 8, while 1.17 and above use Java 17+. I recommend installing both to make it simpler to use different versions of Minecraft whenever you want.

In order to download Java, we will first head to the [Adoptium download page](https://adoptium.net/temurin/releases). Adoptium is an open source Java that does not require a paid account to install, and is made by the Eclipse Foundation, a very reputable source. To install, we will use the dropdown boxes to make it easier to find the versions of Java we need

- Operating System: Windows
- Architecture: x64
- Package Type: JDK or JRE (it does not matter)
- Version: 8 and 17 (download one of them, then download the other after)

Once we have chosen our download preferences, we will click the `.msi` download option. Once it's downloaded, run it and follow the installation process. Do this for both versions of Java.

### Step 2 - Installing Prism

[Download Prism Launcher](https://prismlauncher.org/download). You will most likely want to download the `Installer (.exe)` version. Once it is finished downloading, it may give a warning screen saying "Windows protected your PC". Simply press the "More info" button, then "Run anyway".

Continue the installation process until you get to the "Java" screen. Here, you will decide which Java you want to set as the default for new instances. Click on the version that says "1.8" at the beginning of the version and has "Eclipse Foundation" in the path name. This is your Java 8 and it will be the default version of Java for every new instance you create on Prism. Of course, you can always change this later and can still manually specify a different version of Java whenever you want.

For the Minimum and Maximum memory allocation, leave them at 512 MiB and 4096 MiB respectively, unless you only have 8GB of ram or less, in which case you may want to change the maximum to 2048 MiB.

All of these settings can be later adjusted globally or per instance. This includes changing the Java version or memory allocation. See the global settings button on the main page or in instance settings once you've completed this guide.

After this, continue with the installation process as normal.

### Step 3 - Logging in

Now that we've installed Prism, let's log in. Once Prism has launched, you should see a Steve head and "Profiles" text in the top right. Click on this and press "Manage Accounts". From here, click "Add Microsoft" on the right side menu. This will open a popup window, which will have a button to open the link to verify yourself and also copy the code. Simply paste the code into the window that opens up. Note, you may need to sign in to your Microsoft account first.

Once this is completed, you can exit back to the main Prism Launcher menu. Click on the button at the top left that says "Add Instance".

### Step 4 - Creating an Instance

This guide will focus on Forge 1.8.9, but steps for other versions should also be obvious.

Once you've clicked on the button on the top left that says "Add Instance", name it whatever you want and giving a group for it is optional, but I do not recommend giving a group name until you need to better organize your instances.

Under the `Version` selector, scroll down till you find 1.8.9 and select it. Then in the `Mod Loader` tab directly underneath, choose Forge (NOTE: this is not the tab on the left that says CurseForge). It will automatically choose the latest version of Forge for 1.8.9 for you. Simply click "OK" to proceed. You should now be back on the main Prism page.

### Step 5 - Installing our mods / SkyClient

Now that we've installed Forge 1.8.9, we need to move all our mods to the new Prism Launcher folder. To do that, we'll right click our new instance and press `Edit` to generate the required files, then we exit out of this menu. Now right click the instance and press `Folder` and you should be redirected to a File Explorer window, where you should open the folder titled `.minecraft`. Now, open a new File Explorer by pressing `Win + E` on your keyboard, then navigate to your old .minecraft folder by typing `%appdata%`. Then open the `.minecraft` folder (and if you are using SkyClient, you then need to open the `skyclient` folder). Simply move everything in this folder into the Prism Launcher `.minecraft` folder that you opened earlier. Once this is done, you should be able to see all your mods in the Mods tab, and can launch the instance.

[A quick video guide explaining this process can be found here.](https://youtu.be/DEGaD-_HFCE)

When downloading mods from now on, you can simply drag and drop them into the Mods tab in Prism Launcher. Additionally, if the mod is on Modrinth or CurseForge, you can download them within the launcher using the `Download Mods` button.

### Step 6 - Explore

Prism Launcher has a lot of things to offer, such as themes if you don't like the look of it, as well as a lot of options for your instances, including the ability to see all your mods, resource packs, and worlds in the launcher before launching. You can use these menus to install mods and resource packs, and even update mods if they are hosted on Modrinth or CurseForge! Please take the time to actually learn how the launcher works and experiment with it! Prism is an incredibly powerful launcher and it's important to know exactly what you can do with it!

You can find a list of Prism themes and how to install them on [their website](https://prismlauncher.org/wiki/getting-started/change-themes).

### Step 7 - Updating Prism

Automatic updating has been added since Prism Launcher 8.0. Simply press the `Update` button in the top toolbar to check for updates.

If you are on a version less than 8.0, you will need to download the installer and run it again (you will not lose your instances/your SkyClient).

In some cases (specifically when you are on version 5.x or lower), you may need to uninstall your current Prism Launcher entirely before reinstalling. Your instances will still be safe and will not be deleted.

### Step 8 - Setting CurseForge API Key

Some CurseForge mods may not allow downloads from third party launchers such as Prism Launcher. This can be bypassed by opening Prism settings, going to `APIs`, then `API Keys` and entering `$2a$10$bL4bIL5pUWqfcO7KQtnMReakwtfHbNKh6v1uTpKlzhwoueEJQnPnm` into the CurseForge Core API.

## Common Issues

#### `The java binary "" couldn't be found. Please fix the java path override in the instance's settings or disable it.`

In the main screen of Prism Launcher, click `Settings` near the top, a popup should appear. From here click `Java`, under `Java Runtime` you should click `Auto-detect`, a new popup should appear, listing the java versions. Here you should be given the option to choose the java version that will be used, click on `1.8.0_xxx`(xxx symbolizes the newest version of Java at the time of your installation).

If you do not see any version, [you should redo step 1](#step-1-installing-java)

<br>

#### `This instance is not compatabile with Java version x.`

Click your instance and go to `Edit`. click `Settings` on the left. From here click `Java installation` so that the section is ticked and editable. Click `Auto-detect`, a new popup should appear, listing the java versions. Here you should be given the option to choose the java version that will be used, click on `1.8.0_xxx` (xxx symbolizes the newest version of Java at the time of your installation), or whatever version of Java you want to use such as 17 for newer versions of Minecraft.

If you do not see any version, [you should redo step 1](#step-1-installing-java).

<br>

#### `A problem occured whilst running the Java Virtual Machine. Program will exit.`

Make sure you have selected the x64 version of Java. You can check by clicking on your instance and go to `Edit`, then click `Settings` on the left side. Then, click the `Java installation` checkbox so that the section can be edited. Click `Auto-detect`, and a new popup will appear, with all the Java versions installed. Here, you should be able to see the first part of the path where Java is installed. Ensure that the Java version you have selected starts with `C:\Program Files` and not `C:\Program Files (x86)`.

If you do not see a valid option, [you should redo step 1](#step-1-installing-java)

#### `SkyClient Updater still shows that it failed to update my mods!`

Make sure you have selected a version of Java newer than `1.8.0_51`. Follow the steps in the [This instance is not compatible with Java version x.](#this-instance-is-not-compatible-with-java-version-x.) to fix the issue, but make sure the version is higher than `1.8.0_51`.

#### `My mods arent showing up in-game!`

There are 2 common causes for this, click on the instance once then on the right click `Edit`, then in the next popup click `Mods`.

If you do not see any mods in the mods tab, [you should redo step 5](#step-5-installing-our-mods-skyclient).

If you see a list of mods here then you should click `Version` and on the right click `Install Forge`, the latest version should be highlighted. Click `OK` and Forge should be installed, and the mods should work.

<br>

If you encounter any issues not shown here you should ask for help in my [discord server](https://discord.gg/rejfv9kFJj).
If you encounter any issues **unrelated to the guide at all**, or if you want to be in their community or follow for updates, you can ask in the [Prism Community discord server](https://discord.gg/prism-community-1031648380885147709)

# Contributors

* [PandaNinjas](https://github.com/pandaninjas)
* [Shiggy](https://github.com/Shiggy-dev)
* [KTrain5169](https://github.com/KTrain5169)
