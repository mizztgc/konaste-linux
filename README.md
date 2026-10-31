# Konaste Linux

An unofficial script for playing KONAMI Amusement Game Station (Konaste/コナステ) games on Linux-based operating systems using Wine, written in Bash.

> [!IMPORTANT]
> Konaste Linux is in no way affiliated with, endorsed, nor supported by KONAMI. An active KONAMI ID and the necessary subscriptions ***are required to access the full versions of each game***.

## SUPPORTED GAMES

Konaste Linux can install and launch the following games:

- **beatmania IIDX INFINITAS**
- **SOUND VOLTEX EXCEED GEAR コナステ**
- **DanceDanceRevolution GRAND PRIX**
- **GITADORA コナステ**
- **ノスタルジア**
- **pop'n music Lively**
- **ボンバーガール**

> [!NOTE]
> Only the subscription-based games (and Bomber Girl) are supported with Konaste Linux. The games that are streamed from KONAMI are not yet supported.

For a list of game-specific issues and error codes, see [Game Issues](https://github.com/mizztgc/konaste-linux/wiki/Game-Issues) \& [Error Codes](https://github.com/mizztgc/konaste-linux/wiki/Error-Codes).

## DEPENDENCIES

> [!NOTE]
> The dependency names listed here are their associated packages on **Arch Linux**. Check your distribution's package repositories for the appropriate package(s).

Konaste Linux requires the following dependencies:

* **Web browser of your choice** (needed to launch the games)
* **wine>=9.0** (self-explanatory.)
* **wine-mono** (needed for the launcher's settings menu to function)
* **pipewire** (for sound)
* **pipewire-pulse** (for sound)
  * Debian users may need to also install **pulseaudio-utils**
* **pipewire-audio** (for sound)
* **gst-libav** (for video decoding)
* **gst-plugins-ugly** (necessary for decoding)
* **libpulse** (for sound & to determine audio sample rate)
* **xdg-utils** (to handle the login tokens)
* **wget** (for downloading the needed windows dependencies and of course, the game installers)
* **zenity** (for showing dialog boxes)

### OPTIONAL DEPENDENCIES:

* **msitools** (for silent install via `--silent`)

## HOW TO INSTALL:

### Arch Linux-based Distros (EndeavourOS, Manjaro, CachyOS, etc.)

Konaste Linux can be installed from the [Arch User Repository](https://aur.archlinux.org/packages/konaste-linux). Using an AUR helper such as `yay`, run the following command:

```
yay -S konaste-linux
```

Once installed, run `konaste init` to setup the Wineprefix.

### Other Distributions

> [!WARNING]
> SteamOS is not supported. Aside from it not shipping with some necessary codecs by default, any change you make to the base OS will be reverted every update.

Download the latest archive from [Releases](https://github.com/mizztgc/konaste-linux/releases) and run `install.sh`.

Once installed, run `konaste init` to setup the Wineprefix.

# Special thanks

* [This Reddit thread](https://www.reddit.com/r/bemani/comments/yardc2/anyone_run_their_konasute_infinitas_sdvx_etc/) [(this comment specifically)](https://www.reddit.com/r/bemani/comments/yardc2/comment/ke5z7mi/)
* [Bombergirl on Linux](https://rentry.org/bombergirl-linux) guide
