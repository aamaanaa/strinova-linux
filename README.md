# Strinova on linux
Lutris script and guide to let strinova run on linux. It works by setting a certain registery key, and that seems to manage the conflict the anticheat has with winedbg.

For now this is working. But since it is kernel level anticheat, i hope the devs keep it that way. Since we do not need to modify game files, it seems to me that this is not a reason to be banned, but be warned. it can happen.

- Tested on Fedora 42

## Instructions
- install lutris.
- Download the yaml playbook, and in lutris, select that yaml file and install the game that way
- That is it

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
