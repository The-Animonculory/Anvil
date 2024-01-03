# ANVIL - "The Forge on Which to Create"

![banner image](https://raw.githubusercontent.com/Althro/Anvil/main/Resources/AnvilTestThumbnail.png)

Wabbajack Modlist Installer by Althro with support from Aetherius Modding.

<table stlyle="border: none;">
<tr>
<td><img src="https://raw.githubusercontent.com/Althro/Anvil/main/Resources/WJIcon.png" width="64px" /></td>
<td><a href="https://github.com/wabbajack-tools/wabbajack/releases">Download on Wabbajack</a></td>	
<td><a href="https://loadorderlibrary.com/lists/anvil">View modlist</a></td>
<td><img src="https://raw.githubusercontent.com/Althro/Anvil/main/Resources/AMLogo.webp" width="72px" /></td>
<td><a href="https://discord.gg/aetherius-modding"><img alt="Discord" src="https://img.shields.io/discord/1132691434420576337?style=for-the-badge&label=Aetherius%20Modding"></a></td>
</tr>
</table>

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

## Preamble

**Anvil** is designed as a baseline list to be used as either a forking base for a list or a mod development base. It is fully documented with all changes and tweaks being present in the notes section of MO2, and comes with **two** profiles, aptly named **"Anvil - Forge"** and **"Anvil - Core"**.

**Forge** comes with all the libraries a plugin developer would need and also includes the Creation Kit with [Creation Kit Platform Extended](https://www.nexusmods.com/skyrimspecialedition/mods/71371) configured and working. It serves as the replacement to [Althro's Dev Tools](https://github.com/Althro/ADT).

**Core** is a visual overhaul with an emphasis on "less is more" and improving what is already there. [Community Shaders](https://www.nexusmods.com/skyrimspecialedition/mods/86492) and [ENB](http://enbdev.com/news.html) are present so you can decide which you want to use. It serves as the replacement for [Althro's/Animonculory Visual Overhaul](https://github.com/Althro/Anvil).

## System Requirements

### Disclaimer

Owing to the need to clean master files and certain errors with Wabbajack, Anvil only supports **English Steam** versions of Skyrim SE. **GOG and other Languages are not supported**. The specific version used is 1.6.1130.

Only, Windows 10 and 11 work with Wabbajack fully. LTSC, special variants, lightened editions or any other modified variant **WILL NOT WORK**. Linux compatability is **not possible** at this time owing to certain libraries not present in Wine/Proton required for MO2.

Running the list from Hard Disk Drives or external drives is **STRONGLY ADVISED AGAINST**. A lot of content is swapped at game run time and, as a result, fast storage and RAM are needed.

### Recommended System Requirements

Anvil requires a mid-tier modern system to run to its fullest potential. The recommended specs given below are based on utilizing the ENB in the list. For community shaders, you can subtract a little bit from them.

| Component    | Recommended | 
|:--------------:|:-------------:|
| CPU | 6 core/12 thread
| Ram | DDR4 Ram  + 20GB Pagefile 
| Storage | SSD
| GPU | 6GB VRAM 

Space required: Approx 80GB (Downloads included) + 30GB working room for Wabbajack.

:warning: **NOTE**: AMD RX 580 and older cards are **not supported**. :warning:

## Installation

Installing Anvil is relatively easy and, if you have Nexus Premium, will be a simple waiting game. If you are updating the modlist, you can safely skip to the [updating section](#updating).

### Pre-Installation

Prior to installing Anvil, please complete the following steps.


1. Install [Visual C++ x64](https://aka.ms/vs/16/release/vc_redist.x64.exe) & [.Net Runtime v5 desktop x64](https://dotnet.microsoft.com/download/dotnet/5.0/runtime).
2. Change Skyrim so it does not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
3. Fully uninstall Skyrim by deleting the folder and the Skyrim Special edition folder inside \Documents\My Games\.
4. Fully disable OneDrive and any other programs which hook into user file areas.
5. Reinstall Skyrim into a location that is not Program files. Somewhere like `C:\Games` is a good location. If you only have one drive, look into LostDragonist's [SteamLibrary tool](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide).
6. Start the game once and let it do the graphics check. Do not worry about the settings as it will be replaced during installation. **DO NOT LAUNCH THE GAME TO GET THE CC CONTENT - Anvil requires a totally stock installation.**
7. Install the [Creation Kit on Steam](https://store.steampowered.com/app/1946180/Skyrim_Special_Edition_Creation_Kit/).
8. Run it once and select `NO` when it asks about unpacking scripts. They are handled by ADT already.
9. Close the creation kit and continue with the installation steps.
10. Remove/Disable any 3rd party antivirus such as MalwareBytes or Webroot. These **will** mess with the installation and, in the case of the latter, causes more problems than it solves.

***

### Wabbajack Installation

#### Installing Wabbajack

Once you have completed pre-installation, download the [latest version of Wabbajack]((https://github.com/wabbajack-tools/wabbajack/releases)) and place it in a folder such as `C:\Games\Wabbajack`. Do not place it in program files, on your desktop or in your downloads folder. I recommend placing it on an SSD as it will work quicker on there.

:warning: **NOTE**: Anvil will **always** require the latest version of Wabbajack **UNLESS IT IS SPECIFICALLY STATED HERE**. :warning:

#### Downloading and Installing Anvil

Downloading and installing Anvil can take a while depending on your internet connection and computer. To install Anvil, complete the following steps.

1. Open Wabbajack and click on browse modlists.
2. Press the download button on Anvil and wait for it to download.
3. Set the installation folder to be somewhere like C:\Games\Anvil. **Do not install it to your desktop or downloads folder.**
4. The download location does not need to be on a SSD but it makes installing a bit faster.
5. Press the play button to begin.
6. Go and pet your nearest fluffy animal whilst Wabbajack does its thing. Alternatively read through this readme again.
7. If the installation is successful, jump for joy and move onto [post installation](#post-installation). If the installation is unsuccessful, follow what is below.

***

##### Problems with installation

It is possible that you may encounter an error with Wabbajack when installing. Some common issues are listed below.

- Could not download x:
	- Big files can fail to download due to connection issues. You can either run Wabbajack again or download the file manually. If you decide to manually download it, make sure to place it in the same place as the other downloads.
    - Ensure your version of Curios matches the one used in Anvil. **It has to be the one from Steam, not the one from in-game**.

- x is not a whitelisted download:

	 - This will happen when I update the modlist. Please check if there is a new update or wait until you see a release ping.

- Wabbajack could not find my game folder:

	- Either buy the game or go back to the [Pre-Installation](#pre-installation) step.

- Antivirus reports a virus:
	- You did not follow the steps in [Pre-Installation](#pre-installation). Go back and follow it.
	- If you have followed it then you can fix this by [adding an exclusion for Mod Organizer in Windows Defender](https://www.thewindowsclub.com/exclude-a-folder-from-windows-security-scan).

## Post-Installation

### Stock Game & Root Builder

Anvil utilizes a Wabbajack technology called Stock Game. What this essentially does is create a copy of your Skyrim installation within the installation location of the list. This enables greater compatibility with other mod-lists.

Anvil also utilizes Root Builder alongside Stock Game to enable easier management of hooks such as Reshade and Engine Fixes. Please see our guide to [Root Builder](https://github.com/The-Animonculory/Modding-Resources/blob/main/Root%20Builder%20for%20Skyrim%20AE.md) for more details.
***

### Post Processing

Anvil uses [Wander - A Weather Mod](https://www.nexusmods.com/skyrimspecialedition/mods/24439) with lighting governed by [Relighting Skyim](https://www.nexusmods.com/skyrimspecialedition/mods/8586) & [Enhanced Lighting for ENB](https://www.nexusmods.com/skyrimspecialedition/mods/1377). These are method patched and easy enough to remove should you wish to switch to something else.

[Wandershade](https://www.nexusmods.com/skyrimspecialedition/mods/50045) is included as the ENB and is enabled out of the box. The only change made is to the screenshot format. Again, this is easy to remove/change.

The list also comes with [Community Shaders (CS)](https://www.nexusmods.com/skyrimspecialedition/mods/86492) and all addons required. If you wish to use this, please enable the `Anvil - Core CS` profile.

**NOTE**: Screenshots save to `Overwrite\Game Root`.

**NOTE**: By default, the list is **capped at 82fps**. To change this, you will need to adjust the `ini` file in `SSE Display Tweaks` and disable the framerate lock in ENB if using.

## Playing the List

### Ultrawide Setup

To enable 21x9 ultrawide support, activate the two mods tagged `21x9` under `UI Fixes [Forge & Core]`. **NOTE**: Resolutions outside of 21x9 and 16x9 are **NOT** supported.

### Real-time performance monitoring

Anvil includes a mod that enables you to see your FPS and VRAM usage in real-time. To disable this, deactivate the mod called `OSD Font for SSE Display Tweaks`. **NOTE**: This comes enabled by default.

***

### Starting up the list
Open the installation folder and double-click on the program called `ModOrganizer.exe`. 

Make sure the dropdown box on the right is set to `SKSE` and press the `Run` button.

### In-game MCM options

Anvil has no required MCM options to be selected; however, you can load the smoothcam preset if you wish to do so.

- SmoothCam
	- Load Preset

You are welcome to change any others to achieve your desired setup.

### Starting the Game

By default, Anvil uses [Optional Quick Start](https://www.nexusmods.com/skyrimspecialedition/mods/63953) to bypass the starting sequence of the game and spawn you into the Helgen tunnel. The equipment chest has been custom configured for the list to provide a range of starting equipment.
	
## Updating the modlist

Before updating, please check the changelog and back up your saves. You may need to start a new game after certain updates.

Updating is like installing the list. Simply make sure your paths are the same and tick the `overwrite existing modlist` button. **Note**: Any mods you have added will be deleted when updating.

### Tweaking the Game Settings

#### BethINI

To get some more FPS, tweak the following value in the detail section in BethINI.

- `Shadow Resolution`: 2048
- `Remove Shadows`: I really don’t recommend turning this on, but if you must, then you can.

## Removing the Modlist
Simply delete the folder, and you have uninstalled it.


## Credits and Thanks

- _YOU_ for reading this.
- Ferroxius for the logo, splash and ensuring focus.
- The Aetherius Modding Team.
- The beta testers on Aetherius Modding.
- Noggog for Mutagen.
- xSlim & Aosana for proofreading documentation.
- Umgak for help patching.
- Halgari and everyone on the WJ Team - Wabbajack is awesome and so are you.

## Contact

Whilst I am available primarily on [my server](https://discord.gg/xRrHRsb5e9), please check the [issues](https://github.com/Althro/Anvil/issues) tab on GitHub first if you have any issues. DO NOT DM ME ON DISCORD.
