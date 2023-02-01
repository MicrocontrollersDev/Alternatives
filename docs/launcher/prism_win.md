# Prism Launcher

Recently, the default Minecraft launcher has been having a lot of issues. Almost every week it feels like Mojang manages to break something that causes many people to not be able to play the game. Being a modded version of an already old Minecraft version, I am not too hopeful that many of these issues will ever be fixed or will be fixed anytime soon. For this reason, its recommended to switch to a launcher that cares about modding and old versions of Minecraft, and whose devs we can easily reach out to to report any major issues.

This guide will explain the install process for Prism, as well as how we can use it for Skyclient.

## How to Install (Windows)

- This guide will only be for windows for now. Despite looking long, this is a very simple process and should only take a few minutes! This guide will also assume you are migrating from Skyclient, but steps will be largely the same, except for the migrating data section.

### Step 1 - Installing Java

First, we need to download and setup Java to be able to use Prism Launcher. Unlike the default Minecraft launcher, Prism does not come bundled with a default Java, and so we must install it ourselves.

Minecraft 1.16 and below all use Java 8, while 1.17 and above use Java 17+. I recommend installing both to make it simpler to use different versions of Minecraft whenever you want.

In order to download Java, we will first head to the [Adoptium download page](https://adoptium.net/temurin/releases/). Adoptium is an open source Java that does not require a paid account to install, and is made by the Eclipse Foundation, a very reputable source. To install, we will use the dropdown boxes to make it easier to find the versions of Java we need

- Operating System: Windows
- Architecture: x64
- Package Type: JRE
- Version: 8 or 19 (download one of them, then download the other after)

Once we have chosen our download preferences, we will click the `.msi` download option. Once it's downloaded, run it and follow the installation process. Do this for both versions of Java.

- If on Mac, download the .pkg instead
- If on Linux, download the tar.gz instead

### Step 2 - Installing Prism

[Download Prism Launcher](https://prismlauncher.org/download/). You will most likely want to download the `Installer (.exe)` version. Once it is finished downloading, it may give a warning screen saying "Windows protected your PC". Simply press the "More info" button, then "Run anyway"

Continue the installation process until you get to the "Java" screen. Here, you will decide which Java you want to set as the default for new instances. Click on the version that says "1.8" at the beginning of the version and has "Eclipse Foundation" in the path name. This is your Java 8 and it will be the default version of Java for every new instance you create on Prism. Of course, you can always change this later and can still manually specify a different version of Java whenever you want.

For the Minimum and Maximum memory allocation, leave them at 512 MiB and 4096 MiB respectively, unless you only have 8GB of ram or less, in which case you may want to change the maximum to 2048 MiB.

After this, continue with the installation process as normal.

### Step 3 - Logging in

Now that we've installed Prism, let's log in. Once Prism has launched, you should see a Steve head and "Profiles" text in the top right. Click on this and press "Manage Accounts". From here, click "Add Microsoft" on the right side menu. This will open a popup window, which will have a button to open the link to verify yourself and also copy the code. Simply paste the code into the window that opens up. Note, you may need to sign in to your Microsoft account first.

Once this is completed, you can exit back to the main Prism Launcher menu. Click on the button at the top left that says "Add Instance".

### Step 4 - Creating an Instance

This guide will focus on 1.8.9, but steps for other versions should also be obvious.

Once you've clicked on the button on the top left that says "Add Instance", name it whatever you want and giving a group for it is optional, but I do not recommend giving a group name until you need to better organize your instances.

Under the `Version` selector, scroll down till you find 1.8.9 and select it. Then in the `Mod Loader` tab directly underneath, choose Forge (NOTE: this is not the tab on the left that says Curseforge). It will automatically choose the latest version of Forge for 1.8.9 for you. Simply click "OK" to proceed. You should now be back on the main Prism page.

## Step 5 - Installing our mods

Now that we've installed Forge 1.8.9, we need to move all our mods to the new Prism Launcher folder. To do that, we'll right click our new instance and press `Edit`. Now, we'll go to the `Mods` tab. On the bottom right, there will be a button called `View Folder`. Click on this and you should be redirected to a file explorer tab. Now, open a new file explorer by either pressing `Win + E` on your keyboard or right clicking the file explorer icon and pressing "File Explorer". Navigate to your old .minecraft folder, which is `C:\Users\USER\AppData\Roaming\.minecraft` (change USER to your computer's name, or if you don't know it, press the `Windows` key and `r` at the same time to open up Run, and type `%appdata%` to open your Roaming folder). Open the `.minecraft` file, then open the `skyclient` file if you are using Skyclient. Simply move everything in the skyclient folder into the Prism Launcher .minecraft folder that you opened earlier. Once this is done, you should be able to see all your mods in the Mods tab, and can launch the instance.

[A quick video guide explaining this process can be found here.](https://youtu.be/DEGaD-_HFCE)

### Step 6 - Explore

Prism Launcher has a lot of things to offer, such as themes if you don't like the look of it, as well as a lot of options for your instances, including the ability to see all your mods, resource packs, and worlds in the launcher before launching. You can use these menus to install mods and resource packs, and even update mods if they are hosted on Modrinth or CurseForge!

## Step 7 - Updating Prism

- WIP

## Common Issues

#### `The java binary "" couldn't be found. Please fix the java path override in the instance's settings or disable it.`

In the main screen of Prism Launcher, click `Settings` near the top, a popup should appear. From here click `Java`, under `Java Runtime` you should click `Auto-detect`, a new popup should appear, listing the java versions. Here you should be given the option to choose the java version that will be used, click on `1.8.0_362`.

If you do not see any version, [you should redo step 1](#step-1-installing-java)

You may also need to set the java version in the instance, click on the instance once then on the right click `Edit`, then in the next popup click `Settings` once again click `Auto-detect` and choose the java version.

<br>

#### `My mods arent showing up in-game!`

There are 2 common causes for this, click on the instance once then on the right click `Edit`, then in the next popup click `Mods`.

If you do not see any mods in the mods tab, [you should redo step 5](#step-5-installing-our-mods)

If you see a list of mods here then you should click `Version` and on the right click `Install Forge`, the latest version should be highlighted. Click `OK` and Forge should be installed, and the mods should work.

<br>

If you encounter any issues not shown here you should open a ticket in our [discord server](https://inv.wtf/skyclient/)
