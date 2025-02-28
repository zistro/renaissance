You don't need to. You need to to install MangoHud from Flathub by running:

```
flatpak install mangohud
```

For current Heroic Launcher install version org.freedesktop.Platform.VulkanLayer.MangoHud 23.08

To customize make MangoHud folder in ~/.config and place MangoHud.conf there.

Then run once

```
flatpak override --user --filesystem=xdg-config/MangoHud:ro
```
And tick checkbox in game settings in Heroic Launcher.

