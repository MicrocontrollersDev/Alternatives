# Prism Launcher

Prism Launcher is an incredibly powerful launcher that makes managing your mods and modded instances much easier. It can do everything the official launcher can do, but allows for much more customization and ease of access. The official launcher has had several issues that have taken weeks to fix or are currently still not fixed, despite their severity. For modded and vanilla users alike, it is recommended to switch to Prism Launcher for an issue-less experience.

This guide will explain the install process for Prism, as well as how we can use it for SkyClient. Please take the time after setting up to better learn your way around the launcher, as you may end up using it as your go-to launcher from now on!

## How to Install (Linux)

- This is the install guide for GNU/Linux. Despite looking long, this is a very simple process and should only take a few minutes! This guide will also assume you are migrating from SkyClient, but steps will be largely the same, except for the migrating data section.

### Step 1 - Installing Java

First, we need to download and setup Java to be able to use Prism Launcher. Unlike the default Minecraft launcher, Prism does not come bundled with a default Java, and so we must install it ourselves.

Minecraft 1.16 and below all use Java 8, while 1.17 and above use Java 17+. I recommend installing both to make it simpler to use different versions of Minecraft whenever you want.

In order to download Java, we will first head to the [Adoptium download page](https://adoptium.net/temurin/releases). Adoptium is an open source Java that does not require a paid account to install, and is made by the Eclipse Foundation, a very reputable source. To install, we will use the dropdown boxes to make it easier to find the versions of Java we need

- Operating System: Linux
- Architecture: x64
- Package Type: JDK
- Version: 8 and 17 (download one of them, then download the other after)

Once we have chosen our download preferences, we will click the `tar.gz` download option and install it.

### Step 2 - Installing Prism

[Download Prism Launcher](https://prismlauncher.org/download/linux). Below you will find distro specific instructions on how to download Prism Launcher which you can also find on their website.

<details>
<summary>How do I install Prism Launcher?</summary>
Below you will find distro specific instruction on how to install Prism.
<br>
If you don't know what distro you're using you probably shouldn't be using Linux.
    <details>
    <summary>Flatpak (most distros)</summary>
    <a class="button type-link" href="https://flathub.org/apps/details/org.prismlauncher.PrismLauncher" target="_blank">Install from FlatHub</a>
    </details>
    <details>
    <summary>Alpine Linux</summary>
    <a class="button type-link" href="https://pkgs.alpinelinux.org/packages?name=prismlauncher" target="_blank"> APK Packages</a> are available on Alpine Linux Edge for multiple architectures
    ```bash
    apk add prismlauncher
    ```
    </details>
    <details>
    <summary>Arch Linux</summary>
    There are several AUR packages available:
    <br>
<a class="button type-link" href="https://aur.archlinux.org/packages/prismlauncher" target="_blank">prismlauncher</a>
<br>
<a class="button type-link" href="https://aur.archlinux.org/packages/prismlauncher-bin" target="_blank">prismlauncher-bin</a>
<br>
<a class="button type-link" href="https://aur.archlinux.org/packages/prismlauncher-git" target="_blank">prismlauncher-git</a>
    <details>
    <summary>Installing with an AUR helper</summary>
```bash
# stable source package:
yay -S prismlauncher
# stable binary package:
yay -S prismlauncher-bin
# latest git package:
yay -S prismlauncher-git
```

If you want to use Qt 5 to build the packages instead:

```bash
# stable Qt 5 source package:
yay -S prismlauncher-qt5
# stable Qt 5 binary package:
yay -S prismlauncher-qt5-bin
# latest Qt 5 git package:
yay -S prismlauncher-qt5-git
```

You can replace yay -S with your preferred <a class="button type-link" href="https://wiki.archlinux.org/title/AUR_helpers" target="_blank">AUR helper's</a> install command.
    </details>
    <details>
    <summary>Installation using Chaotic-AUR</summary>
    If you have not already enabled the Chaotic-AUR follow their instructions on <a class="button type-link" href="https://aur.chaotic.cx/" target="_blank">https://aur.chaotic.cx/</a> to enable it.
  
```bash
# stable package:
sudo pacman -S prismlauncher
# latest git package:
sudo pacman -S prismlauncher-git
```

If you want to use Qt 5 to build the packages instead:

```bash
# stable Qt 5 package:
sudo pacman -S prismlauncher-qt5
# latest Qt 5 git package:
sudo pacman -S prismlauncher-qt5-git
```
</details>
</details>
<details>
<summary>CentOS Stream / Fedora / Red Hat Enterprise Linux</summary>
RPM packages are available on <a class="button type-link" href="https://copr.fedorainfracloud.org/coprs/g3tchoo/prismlauncher/ target="_blank">Copr</a> for x86_64 and aarch64.
If you are on an Enterprise Linux distribution (RHEL, CentOS, Rocky, etc.) and do not have the EPEL repositories enabled, please enable them <a  class="button type-link" href="https://docs.fedoraproject.org/en-US/epel/#_el9" target="_blank">here</a>.
<br>
<br>
Nightly builds are updated automatically in the <a class="button type-link" href="https://terra.fyralabs.com/" target="_blank">Terra repository</a> and built on Copr every 24 hours.

```bash
# enables the copr repo
sudo dnf copr enable g3tchoo/prismlauncher
# stable releases
sudo dnf install prismlauncher
# nightly builds
sudo dnf install prismlauncher-nightly
# stable Qt 5 releases
sudo dnf install prismlauncher-qt5
# nightly Qt 5 builds
sudo dnf install prismlauncher-qt5-nightly
```
</details>
<details>
<summary>Debian / Ubuntu</summary>
We use <a class="button type-link" href="https://docs.makedeb.org/" target="_blank">makedeb</a> for our Debian packages.<br>
Several MPR packages are available:
<br>
<a class="button type-link" href="https://mpr.makedeb.org/packages/prismlauncher" target="_blank">prismlauncher</a><br>
<a class="button type-link" href="https://mpr.makedeb.org/packages/prismlauncher-bin" target="_blank">prismlauncher-bin</a><br>
<a class="button type-link" href="https://mpr.makedeb.org/packages/prismlauncher-git" target="_blank">prismlauncher-git</a><br>
<details>
<summary>Installation using Prebuilt MPR (recommended)</summary>

```bash
curl -q 'https://proget.makedeb.org/debian-feeds/prebuilt-mpr.pub' | gpg --dearmor | sudo tee /usr/share/keyrings/prebuilt-mpr-archive-keyring.gpg 1> /dev/null
echo "deb [signed-by=/usr/share/keyrings/prebuilt-mpr-archive-keyring.gpg] https://proget.makedeb.org prebuilt-mpr $(lsb_release -cs)" | sudo tee /etc/apt/sources.list.d/prebuilt-mpr.list
sudo apt update
sudo apt install prismlauncher
```
NOTE: Prebuilt MPR only officially supports Debian 11, Ubuntu 20.04 and Ubuntu 22.04.
</details>
<details>
<summary>Installation using an MPR helper</summary>
Installing <a class="button type-link" href="https://github.com/AFK-OS/una" target="_blank">UNA</a>

```bash
bash <(curl -fsL https://github.com/AFK-OS/una/raw/main/install.sh)

una update
```

Installing Prism Launcher

```bash
# stable source package:
una install prismlauncher
# stable binary package:
una install prismlauncher-bin
# latest git package:
una install prismlauncher-git
```

You can replace una install with your preferred <a class="button type-link" href="https://docs.makedeb.org/using-the-mpr/list-of-mpr-helpers/ target="_blank">MPR helper's</a> install command.
</details>
<details>
<summary>Installation with Pacstall</summary>
Installing <a class="button type-link" href="https://pacstall.dev/" target="_blank">Pacstall</a>

```bash
sudo bash -c "$(curl -fsSL https://git.io/JsADh || wget -q https://git.io/JsADh -O -)"
```

NOTE: Pacstall is unstable on Debian, due to outdated dependencies.
<br>
<br>
Installing Prism Launcher

```bash
# latest git package:
pacstall -I prismlauncher-git
```
</details>
</details>
<details>
<summary>Gentoo</summary>
Ebuilds are available in the official Gentoo repository, under <a class="button type-link" href="https://packages.gentoo.org/packages/games-action/prismlauncher" target="_blank">games-action/prismlauncher</a> and <a class="button type-link" href="https://packages.gentoo.org/packages/games-action/prismlauncher-qt5" target="_blank">games-action/prismlauncher-qt5</a><br>
Note that, for the time being, it is not stabilized, so it's masked for `~amd64` and `~arm64` only.

```bash
sudo emaint sync -a

# If you need to unmask the package, and considering `package.accept_keywords` to be a folder.
echo ">=games-action/prismlauncher-5.0" | sudo tee -a /etc/portage/package.accept_keywords/prismlauncher
# Or do this if you want to build from the latest commit instead of a release
echo "=games-action/prismlauncher-9999 **" | sudo tee -a /etc/portage/package.accept_keywords/prismlauncher

emerge games-action/prismlauncher
```
Have fun! :)
</details>
<details>
<summary>Nix</summary>
A <a class="button type-link" href="https://github.com/PrismLauncher/PrismLauncher/blob/develop/nix/NIX.md" target="_blank">Nix derivation</a> is available.
<br>
Packages are available for all current Nix distributions.
</details>
<details>
<summary>OpenSUSE</summary>
RPM packages are available on the <a class="button type-link" href="https://download.opensuse.org/repositories/home:/getchoo/" target="_blank">Open Build Service</a>.
  
```bash
# add repository (if on leap, replace 'openSUSE_Tumbleweed' with '15.4')
zypper addrepo https://download.opensuse.org/repositories/home:getchoo/openSUSE_Tumbleweed/home:getchoo.repo
# refresh repository cache
zypper refresh
# stable releases (Qt6 version, only for Tumbleweed)
zypper install prismlauncher
# latest builds (Qt6 version, only for Tumbleweed)
zypper install prismlauncher-nightly
# stable releases (Qt5 version, available for Leap and Tumbleweed)
zypper install prismlauncher-qt5
# latest builds (avalible for Leap and Tumbleweed)
zypper install prismlauncher-qt5-nightly
```
</details>
<details>
<summary>Void Linux</summary>
Prism Launcher is available on the official Void repository.

```bash
sudo xbps-install PrismLauncher
```
</details>
</details>
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

Now that we've installed Forge 1.8.9, we need to move all our mods to the new Prism Launcher folder. To do that, we'll right click our new instance and press `Edit` to generate the required files, then we exit out of this menu. Now right click the instance and press `Folder` and you should be redirected to a file explorer window, where you should open the folder titled `.minecraft`. Now, open a new file explorer and navigate to your old .minecraft folder, which is `~/.minecraft`. Then open the `skyclient` folder if you are using SkyClient. Simply move everything in this folder into the Prism Launcher .minecraft folder that you opened earlier. Once this is done, you should be able to see all your mods in the Mods tab, and can launch the instance.

When downloading mods from now on, you can simply drag and drop them into the Mods tab in Prism Launcher. Additionally, if the mod is on Modrinth or CurseForge, you can download them within the launcher using the `Download Mods` button.

### Step 6 - Explore

Prism Launcher has a lot of things to offer, such as themes if you don't like the look of it, as well as a lot of options for your instances, including the ability to see all your mods, resource packs, and worlds in the launcher before launching. You can use these menus to install mods and resource packs, and even update mods if they are hosted on Modrinth or CurseForge! Please take the time to actually learn how the launcher works and experiment with it! Prism is an incredibly powerful launcher and it's important to know exactly what you can do with it!

You can find a list of Prism themes and how to install them on [their website](https://prismlauncher.org/wiki/getting-started/change-themes).

### Step 7 - Updating Prism

Simply update through your package manager, or reinstall it the same way you installed it.

### Step 8 - Setting CurseForge API Key

Some CurseForge mods may not allow downloads from third party launchers such as Prism Launcher. This can be bypassed by opening Prism settings, going to `APIs`, then `API Keys` and entering `$2a$10$bL4bIL5pUWqfcO7KQtnMReakwtfHbNKh6v1uTpKlzhwoueEJQnPnm` into the CurseForge Core API.

## Common Issues

#### `The java binary "" couldn't be found. Please fix the java path override in the instance's settings or disable it.`

In the main screen of Prism Launcher, click `Settings` near the top, a popup should appear. From here click `Java`, under `Java Runtime` you should click `Auto-detect`, a new popup should appear, listing the java versions. Here you should be given the option to choose the java version that will be used, click on `1.8.0_xxx`(xxx symbolizes the newest version of Java at the time of your installation), or whatever version of Java you want to use such as 17 for newer versions of Minecraft.

If you do not see any version, [you should redo step 1](#step-1-installing-java).

<br>

#### `This instance is not compatabile with Java version x.`

Click your instance and go to edit. click `Settings` on the left. From here click `Java installation` so that the section is ticked and editable. Click `Auto-detect`, a new popup should appear, listing the java versions. Here you should be given the option to choose the java version that will be used, click on `1.8.0_xxx` (xxx symbolizes the newest version of Java at the time of your installation).

If you do not see any version, [you should redo step 1](#step-1-installing-java).

<br>

#### `My mods arent showing up in-game!`

There are 2 common causes for this, click on the instance once then on the right click `Edit`, then in the next popup click `Mods`.

If you do not see any mods in the mods tab, [you should redo step 5](#step-5-installing-our-mods-skyclient).

If you see a list of mods here then you should click `Version` and on the right click `Install Forge`, the latest version should be highlighted. Click `OK` and Forge should be installed, and the mods should work.

<br>

#### `A problem occured whilst running the Java Virtual Machine. Program will exit.`

Make sure you have selected the x64 version of Java. You can check by clicking on your instance and go to `Edit`, then click `Settings` on the left side. Then, click the `Java installation` checkbox so that the section can be edited. Click `Auto-detect`, and a new popup will appear, with all the Java versions installed. Here, you should be able to see the first part of the path where Java is installed. 

If you do not see a valid option, [you should redo step 1](#step-1-installing-java)

<br>

#### `SkyClient Updater still shows that it failed to update my mods!`

Make sure you have selected a version of Java newer than `1.8.0_51`. Follow the steps in the [This instance is not compatible with Java version x.](#this-instance-is-not-compatible-with-java-version-x.) to fix the issue, but make sure the version is higher than `1.8.0_51`.

<br>

## Need More Help?

If you encounter any issues not shown here you should ask for help in my [discord server](https://discord.gg/rejfv9kFJj).
If you encounter any issues **unrelated to the guide at all**, or if you want to be in their community or follow for updates, you can ask in the [Prism Community discord server](https://discord.gg/prism-community-1031648380885147709)

# Contributors

* [Shiggy](https://github.com/Shiggy-dev)
* [KTrain5169](https://github.com/KTrain5169)
