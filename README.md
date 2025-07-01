# unity-hackatime

A [Hackatime](https://hackatime.hackclub.com/) plugin for [Unity](https://unity.com).

![image](https://github.com/user-attachments/assets/80f56962-f006-4f65-a48f-bfafec4f4d13)


## About

This is pretty much just Daniel Geo's implementation of hackatime for Unity. Only thing that I did was to add a way to ignore the rate limit errors.

## Installation using the Unity Package Manager (Unity 2019.1+)

The [Unity Package Manager](https://docs.unity3d.com/Packages/com.unity.package-manager-ui@1.8/manual/index.html) (UPM) keeps package contents separate from your main project files.

1. In the Unity Package Manager, click on the plus sign in the top left corner
2. Select "Install package from git URL..."
3. Enter the following line:
   ```
    https://github.com/101zh/unity-hackatime.git?path=/Assets/com.daniel-geo.unityhackatime
    ```
4. Click on the install button

![image](https://github.com/user-attachments/assets/73ef6434-1164-40fe-8c33-c8365f426382)





## Installation using the Unity Package Manager manifest.json (Unity 2018.1+)

1. Modify your project's `Packages/manifest.json` file by adding this line:

    ```json
    "com.daniel-geo.unityhackatime": "https://github.com/101zh/unity-hackatime.git?path=/Assets/com.daniel-geo.unityhackatime"
    ```

    Make sure it's a valid JSON file. For example:

    ```json
    {
        "dependencies": {
            "com.unity.ads": "2.0.8",
            "com.daniel-geo.unityhackatime": "https://github.com/101zh/unity-hackatime.git?path=/Assets/com.daniel-geo.unityhackatime"
        }
    }
    ```

## Installation (all other Unity versions)

If you don't use the Unity Package Manager, you may copy the `Editor` folder from inside `Assets/com.daniel-geo.unityhackatime` into your project's `Assets` folder.

## Setup

1. Run the Unity editor, go to `Window/HackaTime`, and insert your API key (grab one from https://hackatime.hackclub.com/my/wakatime_setup)
2. Press `Save Preferences`
3. Enjoy!

## Usage

The plugin will automatically send heartbeats to HackaTime after the following events:

* DidReloadScripts
* EditorApplication.playModeStateChanged
* EditorApplication.contextualPropertyMenu
* EditorApplication.hierarchyWindowChanged
* EditorSceneManager.sceneSaved
* EditorSceneManager.sceneOpened
* EditorSceneManager.sceneClosing
* EditorSceneManager.newSceneCreated

## Credits
[@Daniel-Geo](https://github.com/Daniel-Geo) - The person who I forked this from\
__Go Check out [@Daniel-Geo's Credits!](https://github.com/Daniel-Geo/unity-hackatime#credits)__
