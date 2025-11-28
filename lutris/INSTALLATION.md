# Guide for Lutris

## 1. Installing launcher

### Manual import in Lutris (Recommended)
- Download the yaml playbook [here](./strinova.yml).
- click the `+` icon in lutris
- Select `Install from a local install script`
- Select the downloaded yaml file
- Follow on screen instructions

After installing the launcher, close the window and run the launcher in Lutris. Please, do not yet launch the game.

## 2. Game installation
> [!WARNING]
> Game installation (and update) and running game may require different wine versions!
> If installation failed (launcher crashes), select `wine-ge-proton-8.26 (Default)` as your runner, wich is the standard runner bundeled with Lutris.

> [!NOTE]
> It is recommend to leave the installation path at the launcher default of: `C:\Strinova\Game`

### Installing the game using launcher
- Well... Login and install the game. If it asks to install webvieuw, simply click skip.

### Import existing installation from Windows

**NOTE that this is untested by me**

- Copy game to `Strinova/Game`
- Open `Strinova/config.ini`
- Change `CurrentGameVersion` to `< current release number >`
- Change `CurrentStage` to `INITSTAGE`

The version will fall out of date over time, copy new value from Windows or start downloading fresh to get current version string

## 3. Launching the game
Change wine runner to one of the below listed for the smoothest game experience:
- [`wine-tkg 10+ staging ntsync`](https://github.com/future-XD/wine-tkg-staging-ntsync-git) *tested, fork of Kron4ek tkg builds*
- [`wine-tkg 10+ staging`](https://github.com/Kron4ek/Wine-Builds/releases/tag/10.10) *tested, NTSYNC build optional only if ur kernel supports it*

...or any other third party `wine-10+` *not tested by repository maintainers*
 
