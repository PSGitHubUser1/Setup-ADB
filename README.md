## * ⛔Requirements⛔
- Android 11 or later (+)
- API level 31 or later (+)
- A PC / Laptop with Windows 7 or later (+)

## # Download 
- Windows:  [platform-tools_r34.0.5-windows.zip](https://github.com/PSGitHubUser1/setup-adb-windows/files/13843910/platform-tools_r34.0.5-windows.zip)
- MacOS:    [platform-tools_r34.0.5-darwin.zip](https://github.com/PSGitHubUser1/setup-adb-windows/files/13843917/platform-tools_r34.0.5-darwin.zip)
- Linux:    [platform-tools_r34.0.5-linux.zip](https://github.com/PSGitHubUser1/setup-adb-windows/files/13843936/platform-tools_r34.0.5-linux.zip)

## $ 🔧setup-adb🔧

- First open:
 > Settings > Search on top > About Phone / About your Phone > Tap on *Build* (eg. MIUI) version for 7-8 times. And you will become a developer. 
- Go back and search `Developer options` or Scroll down and tap on Additional settings > Developer options
- Click on it and scroll down to turn on `USB debugging` not the `USB debugging (Security settings)`
- Check all things and turn it on.
- And also turn on `Install via USB` (optional)
- Connect your mobile with PC. (Here, I am telling about Windows)
- Download the Platform Tools file from website [here](https://developer.android.com/studio/releases/platform-tools).
- Extract it and open the folder
- Now follow this
---
https://user-images.githubusercontent.com/90406016/219314065-d3c02295-403a-41f2-99d7-1ec839953ab6.mp4

---
- Type this
```cmd
adb devices
```
- If it shows some Alphabets and numbers under 'List' (like AFG485GT..) then your phone is sucessfully connected to PC already.
- Finally you can run any command. Which you want to run. 

## Here's an example
In **`Android 12`** version, [Specifically, POCO phones] have a green coloured icon of camera & mic on Status Bar at the top of screen whenever you use your mic/camera. Which looks nice at first but not forever. here's an img where the camera is being used and this icon occurs:

![File](https://user-images.githubusercontent.com/90406016/219318411-77ba8622-17ed-4038-9b3f-79b843a44b65.png)

- To remove the green icon, you can run this `Android 12`: 
```cmd
adb shell cmd device_config put privacy camera_mic_icons_enabled false default
```
- To revert back [Enable it again]:
```cmd
adb shell cmd device_config put privacy camera_mic_icons_enabled true default
```

### This is how you can setup the `adb`



