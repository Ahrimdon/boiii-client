# BOIII Client

[![discord](https://img.shields.io/endpoint?url=https://momo5502.com/iw4x/members-badge.php)](https://discord.gg/sKeVmR3)
[![website](https://img.shields.io/badge/Repackers-_Website-blue)](https://rimmyscorner.com/)

<p align="center">
  <img src="assets/github/banner-boiii.png?raw=true" />
</p>

## Prerequisites: Installing Git (Optional)

If you don't have `git` installed on your machine, follow these steps:

1. Visit the [Git download page](https://git-scm.com/downloads).
2. Download the appropriate version for your operating system.
3. Run the installer.
   - During the installation, you will be asked if you want to add Git to your system's PATH environment variable. Ensure you choose the option to do so. This allows you to use Git from the command line without specifying its full path.
4. After installation, open a terminal or command prompt and type `git --version` to ensure Git is correctly installed.

## Download
Clone the Git repository or download as ZIP.

- **Clone the repository:**
  - Open a terminal or command prompt.
  - Run the following command:
    ```
    git clone https://github.com/Ahrimdon/boiii-client.git
    ```
- **Download ZIP**
  - Click on the green button at the top of the repo labeled `Code`
  - Click `Download ZIP`


## Repository Contents
  - BOIII Client
  - All Necessary Files (Including `ext.dll`)
  - BOIII Client Dedicated Server Configuration Files

## Added Features
  - Removed BOIII Watermark
  - No Auto-Update
  - Reverted launcher to the original style
  - Changed executable icon to match original

## Installation

### Clients

1. Place the executable `boiii.exe` in your `Call of Duty Black Ops III` directory.
    > **Note**: Usual location is `C:\Program Files (x86)\Steam\steamapps\common\Call of Duty Black Ops III`
2. Place the `boiii` folder into your Local AppData.
    > **Note**: On Windows, press `Win + R`, type `%localappdata%`, click ok.
3. Launch `boiii.exe`

# T7 Server Config
Config for T7 Dedicated Servers for use with the BOIII Client.

## How to use
1. Download the BO3 Unranked Dedicated Server via Steam (It's located in the "Tools" section in your steam library.)
2. Open the Unranked Server folder in windows explorer (if you own BO3 on Steam and have it installed it will be in your BO3 Game Folder)
3. Add boiii.exe to the UnrankedServer Folder
4. Download this repository and extract startup batch files as well as the boiii and zone folder to the UnrankedServer Folder
5. Edit the config(s) in /zone to your liking.
6. (Optional) Edit your game rules under boiii/gamesettings/mp.
6. Port forward UDP 27017.
7. Start the Server using !start_mp_server.bat or !start_zm_server.bat

## Additional Steps required for hosting Zombies Dedicated Servers
As of right now you need to take additional Steps to host Zombies Servers.
For Zombie Dedis to work they need to have the Zombies Maps and common FastFiles, these do not come with the UnrankedServer Files. This means you need to copy those over from your installed BO3 game folder.

Copy common fastfiles that is needed for zombies.

```
zone/en_zm_patch.ff
zone/en_zm_common.ff
zone/zm_patch.ff
zone/zm_common.fd
zone/zm_common.ff
zone/zm_levelcommon.ff
```

Now for the map. Shadows of Evil is zm_zod. 

```
zone/en_zm_zod.ff
zone/en_zm_zod_patch.ff
zone/zm_zod.ff
zone/zm_zod_patch.ff
```

from your BO3 Game folder into the UnrankedServer's ```zone``` Folder. Do the same with the FastFiles of the Maps you want to host on the Server, you do not need to copy the .xpak files, those hold Textures and Sounds which the Server doesn't need. You can use the zm_server.cfg as a short name references if you want to grab the others.

You are now ready to start the Server using !start_zm_server.bat. If the server still instantly closes while opening the !start_zm_server.bat or !start_cp_server.bat. Check the console_mp.log from identities\dedicatedpc\ folder. Scroll down until you see "Could not find zone: xxxx".

## Disclaimer

This software has been created purely for the purposes of
academic research. It is not intended to be used to attack
other systems. Project maintainers are not responsible or
liable for misuse of the software. Use responsibly.