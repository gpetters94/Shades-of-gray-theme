# Shades-of-gray

Shades-of-gray is a flat dark GTK-theme with ergonomic contrasts. It supports *Gnome*, *Cinnamon*, *Xfce4*, *Mate* and *Openbox*.
Theme customizations for *Firefox*, *Thunderbird* and *Inkscape* are additionally included.
Shades-of-gray is available in seven color variants:

<p align="center">
<img src="https://user-images.githubusercontent.com/22373662/52785146-9153ff80-3057-11e9-9d0a-a285ffc32732.png" width="60%"></img></br><i>Gray, Arch, Cerulean, Firebrick, Harvest, Orient, Patina</i>
</p>

The following description with further information is part of the file `Shades-of-gray-Readme.html`, contained in the Shades-of-gray theme folder.

## Table of Contents

- [Installation](#installation)
  - [Arch Linux](#arch-linux)
  - [Installation via terminal](#installation-via-terminal)
  - [Manual Installation](#manual-installation)
- [Gadgets](#gadgets)
  - [Thunderbird](#thunderbird)
  - [Firefox](#firefox)
  - [Inkscape](#inkscape)
  - [Syntax Highlighting](#syntax-highlighting)
- [Requirements](#requirements)
- [License](#license)
- [Screenshots](#screenshots)

## Installation

### Arch Linux

You can install the AUR package:
* Last release: [gtk-theme-shades-of-gray](https://aur.archlinux.org/packages/gtk-theme-shades-of-gray)
* Git version: [gtk-theme-shades-of-gray-git](https://aur.archlinux.org/packages/gtk-theme-shades-of-gray-git)

If you want to benefit from the latest upstream changes, it makes sense to install the Git version.
In *GitHub* [commits](https://github.com/WernerFP/Shades-of-gray-theme/commits/master) you can check if there are changes since the latest release that can be useful for you.

### Installation via terminal

You can install the Git version by using this method:

```
mkdir ~/Shades-of-gray-git
cd ~/Shades-of-gray-git/
git clone https://github.com/WernerFP/Shades-of-gray-theme.git
cd Shades-of-gray-theme/
rm -rf README.md LICENSE .git
sudo cp -r * /usr/share/themes/
```
> **Note:** existing installations of Shades-of-gray are overwritten by the last command. If Shades-of-gray was previously installed using your distribution‘s package management, the package should be uninstalled first.

### Manual Installation

Copy the chosen theme folders either for personal use into directory `~/.themes/` or for common use into `/usr/share/themes/`.

*Shades-of-gray* can also be downloaded from [openDesktop.org](https://www.opendesktop.org/p/1244058/).

## Gadgets

Each theme folder contains an `app-gadgets` directory with additional theme files for *Thunderbird*, *Firefox* and *Inkscape*.

### Thunderbird

The folder `assets` and the file `userChrome.css` in folder `../app-gadgets/Thunderbird-Shades-of-gray/` contain a *Thunderbird* theme adapted to *Shades of gray*. To use these customizations, you can copy both to this location:
```
~/.thunderbird/<name-of-your-profile>/chrome/assets
~/.thunderbird/<name-of-your-profile>/chrome/userChrome.css
```

Select the default theme in the *Thunderbird* settings to ensure a consistent appearance.

#### • Thunderbird Calendar

*Thunderbird‘s* Calendar (formaly *Lightning*) is using its own bright colors in default setting. The option for using theme colors is hidden as '*Accessibility*'.
Open the *Thunderbird* settings and activate the checkbox '*Optimize colors for accessibility*' in calendar area.

> **Note:** Thunderbird 68.0: There are several bugs in the new Calendar (Lightning) - e.g. events are sometimes not visible in the "*Today Pane*". These problem can be handled by deleting the cache folder `/.cache/thunderbird` before starting Thunderbird (see also *Shades-of-gray-Readme.html*).

### Firefox

The directory `../app-gadgets/Firefox-Shades-of-gray` contains a collection of *Shades-of gray* theme modifications for *Firefox*:

* **userChrome.css**</br>
This file contains modifications for the *Firefox* user interface.

* **userContent.css**</br>
Herein are adjustments of the Firefox *Home-Screen*. In addition, the following customizations are imported via `userContent.css`:

* **about.css**</br>
The file `about.css` contains *Shades-of-gray* theme customizations for *Firefox* `about:` pages.

* **bookmark-search-plus-2.css**</br>
The file `bookmark-search-plus-2.css` contains a theme adaption for the very useful add-on *Bookmark search plus 2* ([AMO](https://addons.mozilla.org/firefox/addon/bookmark-search-plus-2) | [Github](https://github.com/aaFn/Bookmark-search-plus-2)).

* **panorama-tab-groups.css**</br>
This is a modification for the dark theme of the recommended add-on *Panorama Tab Groups* ([AMO](https://addons.mozilla.org/firefox/addon/panorama-tab-groups) | [Github](https://github.com/projectdelphai/panorama-tab-groups)).

* **bookmarked-speed-dial.css**</br>
*Bookmarked Speed Dial* ([AMO](https://addons.mozilla.org/firefox/addon/bookmarked-speeddial)) is an underrated add-on that offers similar functionality to *Vivaldi Speed Dial*. The file `bookmarked-speed-dial.css` is a *Shades-of-gray* theme customization.
The folder `bookmarked-speed-dial-images` contains images wich you can choose as '*Default dial image*' and '*Default folder image*' in the add-on options.

To use the customizations for *Firefox* you can copy the contents of directory `../app-gadgets/Firefox-Shades-of-gray/` to this location:

`~/.mozilla/firefox/<name-of-your-profile>/chrome/`

> **Note:** you should choose the dark style in Firefox to get a consistent dark appearance.

> **Note:** as of Firefox 68/69, you must set the `toolkit.legacyUserProfileCustomizations.stylesheets` preference to `true` in `about:config` in order to load `userChrome.css` and `userContent.css` files.

### Inkscape

Original colored icons in *Inkscape* are hard to identify in dark themes. The file `icon.svg` in folder `Inkscape-icons` contains bright icons.
To use them in *Inkscape*, the file must be stored in this directory:

`~/.config/inkscape/icons/icons.svg`

> **Note:** not all symbols can be customized because Inkscape is partly using standard GTK symbols ([&#x1f41e;](https://bugs.launchpad.net/inkscape/+bug/789804)).

### Syntax Highlighting

*Shades-of-gray* includes the syntax color scheme *Shades-of-pastel* for several editors. By using pastel colors on dark background like pastel chalks on a blackboard the *Shades-of-pastel* scheme provides balanced and easy on eyes contrasts. A set of previews is available in this separate [Shades-of-pastel](https://github.com/WernerFP/Shades-of-pastel) repository.

<p align="center">
<img src="https://user-images.githubusercontent.com/22373662/52785609-ad0bd580-3058-11e9-99c1-13c802444149.png" width="773px" height="158px"></img></br><i>Shades of pastel: Bash sample in Sublime Text</i>
</p>

#### • Sublime Text

To install the scheme for S*ublime Text* change to directory <code>Shades-of-gray/app-gadgets/Syntax-Colors</code>. Copy the contained file <code>Shades-of-pastel.tmTheme</code> to a folder in your *Sublime* Packages directory:
```
mkdir -p $HOME/.config/sublime-text-3/Packages/Shades-of-pastel
cp Shades-of-pastel.tmTheme $HOME/.config/sublime-text-3/Packages/Shades-of-pastel/
```
Now you can select the syntax color scheme *Shades-of-pastel* in menu *Preferences*.

#### • Gedit, Pluma, Xed, Mousepad

*Shades-of-pastel* can be used by editors with syntax highlighting based on *GtkSourceView 3* or *GtkSourceView 4*. To install the color scheme change to directory `Shades-of-gray/app-gadgets/Syntax-Colors`. Copy the contained file `shades-of-pastel.xml` into the following user directories:
```
mkdir -p $HOME/.local/share/gtksourceview-3.0/styles
cp shades-of-pastel.xml $HOME/.local/share/gtksourceview-3.0/styles/

mkdir -p $HOME/.local/share/gtksourceview-4/styles
cp shades-of-pastel.xml $HOME/.local/share/gtksourceview-4/styles/
```
*Shades-of-pastel* is now available in the settings of your editor.

#### • Vim, GVim

To install *Shades-of-pastel* for *Vim* change to directory `Shades-of-gray/app-gadgets/Syntax-Colors`. Copy the file `shades-of-pastel.vim` into your *Vim* profile folder:</p>

```
mkdir -p $HOME/.vim/colors
cp shades-of-pastel.vim $HOME/.vim/colors/
```
Turn on syntax highlighting (`syntax on`) in your configuration file (`~/.vimrc`) and append the line `colorscheme shades-of-pastel` if you want to use the *Shades-of-Pastel* scheme by default.

## Requirements

* GTK+ 3.20 or above
* Pixmap theme engine
* Murrine theme engine

## License

GNU General Public License v3.0

## Screenshots

Cinnamon Patina, Gnome Gray,</br>
Openbox Arch, Xfce4 Cerulean
<p align="center">
<img src="https://user-images.githubusercontent.com/22373662/52785526-8057be00-3058-11e9-8b1f-fa75701b3d1d.jpg" width="45%"></img>  <img src="https://user-images.githubusercontent.com/22373662/52785560-91083400-3058-11e9-93d0-f9fbae247833.jpg" width="45%"></img>  <img src="https://user-images.githubusercontent.com/22373662/52785587-9e252300-3058-11e9-8231-34429b392dbf.jpg" width="45%"></img>  <img src="https://user-images.githubusercontent.com/22373662/52785477-628a5900-3058-11e9-803f-9c75bc6535b0.jpg" width="45%"></img>
</p>
