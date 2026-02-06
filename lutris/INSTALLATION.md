> [!WARNING]
> Game installation (and update) and running game may require different wine versions!
> If installation failed (launcher crashes), select `wine-ge-proton-8.26 (Default)` as your runner, wich is the standard runner bundeled with Lutris.

> [!NOTE]
> It is recommend to leave the installation path at the launcher default of: `C:\Strinova\Game`

> [!WARNING]
> Any other proton version other then protonDW for playing the game will no longer work, see https://github.com/aamaanaa/strinova-linux/issues/43

# Guide for Lutris

## 1. Installing launcher

### Manual import in Lutris (Recommended)
- Download the yaml playbook [here](./strinova.yml).
- click the `+` icon in lutris
- Select `Install from a local install script`
- Select the downloaded yaml file
- Follow on screen instructions

After installing the launcher, close the window and run the launcher in Lutris. Please, do not yet launch the game, as this will fial due to anticheat requirements in the wine runner.

## 2. Game installation

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
Change wine runner to one of the below listed to start playing the game:
- ~~[`wine-tkg 10+ staging ntsync`](https://github.com/future-XD/wine-tkg-staging-ntsync-git)~~ *No longer works*
- ~~[`wine-tkg 10+ staging`](https://github.com/Kron4ek/Wine-Builds/releases/tag/10.10)~~ *No longer works*
- [`ProtonDW`](https://github.com/Vysp3r/ProtonPlus) *Tested and confirmed working* 

> [!TIP]
> Successfully launched the game? Take a moment and [report your hardware](https://github.com/aamaanaa/strinova-linux/issues/new/choose)
