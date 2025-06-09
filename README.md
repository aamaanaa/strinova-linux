![strinova-17sub-2131408368](https://github.com/user-attachments/assets/e8663167-a843-4d3c-ac27-1e17c3a75cfc)


# Strinova on linux
Lutris script and guide to let strinova run on linux. It works by setting a certain registery key, and that seems to manage the conflict the anticheat has with winedbg.

For now this is working. But since it is kernel level anticheat, i hope the devs keep it that way. Since we do not need to modify game files, it seems to me that this is not a reason to be banned, but be warned. it can happen.

- Tested on Fedora 42, with a AMD gpu.

## Instructions
- install lutris.
- Download the yaml playbook, and in lutris, select that yaml file and install the game that way
- That is it

## From the lutris website
The yaml file in this repo has been published by me to the official lutris website. You can find it here:
- https://lutris.net/games/install/39289/view

click the `+` icon in lutris, `Searh the lutris site for installers`.

![Screenshot From 2025-06-09 13-17-38](https://github.com/user-attachments/assets/b6ff294b-8465-45a5-8a21-0b664ef5cb7f)


## Manually import game
if you have the game already installed somewhere else and you want to import it to lutris:

- Copy game to drive_c/Strinova/Game
- In `drive_c/Strinova/config.ini` change CurrentGameVersion to `1.3.10.21` and `CurrentStage` to `INITSTAGE`. The version will fall out of date over time, copy new value from Windows or start downloading fresh to get current version string.

`drive_c/Strinova/config.ini` can be found by right clicking Strinova in lutris > Browse Files

## Notes
It may be required to start the game with a Wine version of at least 10.0+ (wine-tkg is tested).
A crash window will appear. Ignore it. Do not click any of the buttons in the crash window — if you do, the game will crash.
    
Afther the installer is done, download the entire game, and afther that set the wine runner to wine-tkg 10 +. 

It may be needed to set the wine runner to a lower version due the launcher crashing when downloading. It appears that wine-ge-proton-8.26 works.

Game can be played on NVIDIA GPU with some graphical issues [1]

1. https://github.com/ValveSoftware/Proton/issues/8262#issuecomment-2953691047

## Video guide
you may follow this youtube turtorial [2] i have made to install it manually:
2. https://www.youtube.com/watch?v=ylbCdFw0ACU

## Issues and help
please report issues and help in the repo. Please attach the lutris debug log, aswell info of what os you use, what wine runner, what gpu, and so on.

## Additional info
See the reddit discussion [3] i started for usefull info:
3. https://www.reddit.com/r/linux_gaming/comments/1l31uvj/psa_strinova_works/
