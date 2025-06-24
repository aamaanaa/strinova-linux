# Video Guide: https://www.youtube.com/watch?v=tTXlXtChcfc
# Text Guide


## 1. Downloading the Launcher
- Visit the strinova website and download the PC client (non-steam, non-epic games)

## 2. Setting up bottles
- Open Bottles 

### 2.1 Installing the `kron4ek-wine-10.10-staging-tkg-amd64` runner
- Click the hamburger menu on the right then click preferences
- Click runners > Kron4ek > Download `kron4ek-wine-10.10-staging-tkg-amd64`
- If you do not see the runners go to General > Advanced > Enable Pre-Release versions of runners
- Close out of preferences

### 2.2 Creating a bottle
- Click the plus button in the top left corner of bottles
- Select Gaming optimized
- Select the `kron4ek-wine-10.10-staging-tkg-amd64` runner

### 2.3 Configuring the bottle
- Click the newly created bottle
- Click dependencies, scroll down and install `vcredist2022`
- Click settings, 
    - DLL Overrides add `tdh.dll`. Hit enter.
    - In the drop-down next to `tdh.dll` select `Native (Windows)`.
    - Click Environment Variables and add `PULSE_LATENCY_MSEC=60`. Hit enter.
- Click Tools > Registry Editor and navigate to `HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\AeDebug`
- Set `Auto` to `0` and `Debugger` to `` (empty).

## 3. Installing Strinova
- Click run executable and select the game installer (PC client only)
- Click install and use the defaults
- Open the Launcher if prompted
- If asked for the WebView2 install, proceed with the installations. You can uncheck the Bing Bar.
- Once done, click add shortcut and select `drive_c/Strinova/Strinova.exe`
- Hit play and download and install Strinova. It may crash several times. Simply ensure all bottles processes are closed and that winedevice.exe is closed too (it likes to persist even when Bottles is closed).

## 4. Playing Strinova
- Run the Strinova Launcher and hit play just like you would on Windows.
- If you are unable to click on anything, try hitting alt+enter and/or moving the Window to another screen.