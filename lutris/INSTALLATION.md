# Guide

## 1. Installing launcher
> [!NOTE]
> Recommend to leave installation path `C:\Strinova`

~~### Install from Lutris website~~
Not recommended, because of these reasons:
- the lutris team made a mistake and messed up the script and gave wrong copyright
- it can not be updated, since the time taken to approve it on thier websites takes way way to long.

### Manual import in Lutris (Recommended)
- Download the yaml playbook [here](./strinova.yml).
- click the `+` icon in lutris
- Select `Install from a local install script`
- Select the downloaded yaml file
- Follow on screen instructions

### After installing
After installing the launcher, close the window and run the launcher in Lutris

## 2. Game installation
> [!WARNING]
> Game installation(and update) and running game may require different wine versions!
> If installation failed (launcher crashes), select `wine-ge-proton-8.26` as your runner

> [!NOTE]
> Recommend to leave installation path `C:\Strinova\Game`

### Installing the game using launcher
- Well... Login and install the game

### Import existing installation from Windows
- Copy game to `Strinova/Game`
- Open `Strinova/config.ini`
- Change `CurrentGameVersion` to `< current release number >`
- Change `CurrentStage` to `INITSTAGE`

The version will fall out of date over time, copy new value from Windows or start downloading fresh to get current version string


## 3. Launching the game
Change wine runner to listed below
- `wine 10.7 staging` *tested*
- [`wine-tkg 10.4 staging ntsync`](https://github.com/future-XD/wine-tkg-staging-ntsync-git) *tested*
- [`wine-tkg 10.10 staging ntsync`](https://github.com/Kron4ek/Wine-Builds/releases/tag/10.10) *tested*

...or any `wine-tkg 10.X staging` *not tested by repository maintainers*

> [!TIP]
> Successfully launched the game? Take a moment and [report your hardware](https://github.com/aamaanaa/strinova-linux/issues/new/choose)
