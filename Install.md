# Installing Cine Light Match

Install the plugin from Fab or copy it into your project, enable it, restart Unreal, and click the Cine Light Match button on the toolbar.

### Requirements

| Item | Requirement |
| --- | --- |
| Unreal Engine | 5.8 |
| Operating system | Windows 64-bit or macOS (Apple silicon and Intel) |
| Project type | Blueprint-only or C++ |
| Other plugins | Sun Position Calculator (built into Unreal, enabled automatically) |

### Install from Fab

1. Open the Epic Games Launcher and go to your Fab library.
2. Find Cine Light Match and choose to install it to your engine. Pick Unreal Engine 5.8.
3. Open your project and go to **Edit > Plugins**.
4. Search for **Cine Light Match**, tick its checkbox, and restart Unreal when asked.

Installing to the engine makes the plugin available to every project, but you still must enable it per project.

### Install manually into one project

Use this if you received the plugin as a download rather than through Fab.

1. Make sure Unreal is closed.
2. In your project folder, create a folder named `Plugins` if it doesn't already exist.
3. Copy the `CineLightMatch` folder into it, so you have `YourProject/Plugins/CineLightMatch`.
4. Open the project. The plugin should be enabled automatically. If not, enable it in **Edit > Plugins** and restart the project.

The download includes prebuilt files for Windows and Mac, so you don't need a compiler.

### Open the panel

There are two ways to open Cine Light Match:

- Click the **Cine Light Match** button on the level editor toolbar, next to the Play controls.
- Choose **Tools > Cine Light Match** from the main menu.

The panel opens as a tab. Drag it anywhere to dock it; Unreal remembers where you put it.

### About Sun Position Calculator

Cine Light Match uses Unreal's built-in Sun Position Calculator to place the sun from a location, date, and time. Unreal enables it automatically when you enable Cine Light Match. Leave it enabled; turning it off disables sun placement.

### Try it out

1. Open the panel.
2. Look through the camera preset list and try a few sort options.
3. Adjust your viewport to an angle you'd like to create a camera.
4. Pick a preset and click **Create Camera**. A cine camera with the chosen specifications should appear in your level at your current viewport angle. Cameras and lights the plugin created are ordinary Unreal actors and stay in your levels.

### Troubleshooting

| Problem | Fix |
| --- | --- |
| No toolbar button or menu entry | Enable the plugin in **Edit > Plugins**, then restart Unreal. |
| Unreal asks to rebuild missing modules | Your engine version doesn't match the plugin. Install the version built for your engine. |
| Output Log says the widget couldn't be found | The plugin's Content folder is missing. Reinstall the plugin. |
| Sun placement doesn't work | Make sure Sun Position Calculator is enabled in **Edit > Plugins**. |
| Preset list is empty | Check the Output Log for `LogCineLightMatch` warnings and reinstall if the preset table is missing. |

Cine Light Match uses its own copies of all shared Cine Tools code, so it works with or without other Cine Tools plugins installed.
