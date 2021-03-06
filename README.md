# Shades-of-gray

Shades-of-gray is a flat dark GTK-theme with ergonomic contrasts. It supports Gnome, Cinnamon, Xfce4, Mate and Openbox.
Theme customizations for Firefox, Thunderbird and Inkscape are additionally included.
Shades-of-gray is available in seven color variants:

<p align="center">
<img src="https://user-images.githubusercontent.com/22373662/52785146-9153ff80-3057-11e9-9d0a-a285ffc32732.png" width="60%"></img></br><i>Gray, Arch, Cerulean, Firebrick, Harvest, Orient, Patina</i>
</p>

The following description with further information is part of the file `Shades-of-gray-Readme.html`, contained in the Shades-of-gray theme folder.

## Installation

### Arch Linux

You can install the AUR package:
* Last release: [gtk-theme-shades-of-gray](https://aur.archlinux.org/packages/gtk-theme-shades-of-gray)
* Git version: [gtk-theme-shades-of-gray-git](https://aur.archlinux.org/packages/gtk-theme-shades-of-gray-git)

If you want to benefit from the latest upstream changes, it makes sense to install the Git version.
In GitHub [commits](https://github.com/WernerFP/Shades-of-gray-theme/commits/master) you can check if there are changes since the latest release that can be useful for you.

### Installation via terminal

You can install the git version by using this method:

```
mkdir ~/Shades-of-gray-git
cd ~/Shades-of-gray-git/
git clone https://github.com/WernerFP/Shades-of-gray-theme.git
cd Shades-of-gray-theme/
rm -rf README.md LICENSE .git
sudo cp -r * /usr/share/themes/
```
> **Note:** Existing installations of Shades-of-gray are overwritten by the last command. If Shades-of-gray was previously installed using your distribution‘s package management, the package should be uninstalled first.

### Manual Installation

Copy the chosen theme folders either for personal use into directory `~/.themes/` or for common use into `/usr/share/themes/`.

Shades-of-gray can also be downloaded from [openDesktop.org](https://www.opendesktop.org/p/1244058/).

## Gadgets

Each theme folder contains an `app-gadgets` directory with additional theme files for Thunderbird, Firefox and Inkscape.

### Thunderbird

The folder `assets` and the file `userChrome.css` in folder `Thunderbird-Shades-of-gray` contain a Thunderbird theme adapted to Shades of gray. Copy both to this location:
```
~/.thunderbird/<name-of-your-profile>/chrome/assets
~/.thunderbird/<name-of-your-profile>/chrome/userChrome.css
```

If you change a Shades-of-gray theme color, it is not necessary to copy the file again. You can simply comment the current theme color in `userChrome.css` (Thunderbird and/or Firefox) and uncomment the new theme color value.

#### • Thunderbird Calendar

Thunderbird‘s Calendar (formaly Lightning) is using its own bright colors in default setting. The option for using theme colors is hidden as '*Accessibility*'.
Open the Thunderbird settings and activate the checkbox '*Optimize colors for accessibility*' in calendar area.

### Firefox

##### • userChrome.css

The file `userChrome.css` in folder `Firefox-Shades-of-gray` contains a theme adaptation to Shades-of-gray. To enable the customizations, copy the file or its content to this location:

`~/.mozilla/firefox/<name-of-your-profile>/chrome/userChrome.css`

Additional options are included at the end of the file userChrome.css (e.g. to hide unwanted items in context menus). You can activate options of your choice by removing the comment characters `/*` at the beginning of a line.

> **Note:** You should choose the dark style in Firefox to get a consistent dark appearance.

##### • userContent.css

Firefox uses widgets of the current GTK3 theme in websites that have not designed their own widgets for forms. With dark themes this is ugly and input fields, checkboxes etc. are difficult to use (e.g. black font in dark input fields). To fix this behavior the file `userContent.css` contains color-neutral form widgets.

This file also contains theme customizations for the New Tab page (*about:newtab*).

Copy the file or its contents to this location for enabling:

`~/.mozilla/firefox/<name-of-your-profile>/chrome/userContent.css`

### Firefox add-ons

#### • Bookmark search plus 2

The file `bookmark-search-plus-2.css` contains theme customizations for the very useful add-on *Bookmark search plus 2* ([AMO](https://addons.mozilla.org/firefox/addon/bookmark-search-plus-2) | [Github](https://github.com/aaFn/Bookmark-search-plus-2)). Copy this file in addition to `userContent.css` into your *chrome* directory:

`~/.mozilla/firefox/<name-of-your-profile>/chrome/bookmark-search-plus-2.css`

#### • Panorama Tab Groups

The file `panorama-tab-groups.css` contains theme customizations for the recommended add-on *Panorama Tab Groups* ([AMO](https://addons.mozilla.org/firefox/addon/panorama-tab-groups) | [Github](https://github.com/projectdelphai/panorama-tab-groups)). Copy this file in addition to `userContent.css` into your *chrome* directory:

`~/.mozilla/firefox/<name-of-your-profile>/chrome/panorama-tab-groups.css`

> **Note:** In *Panorama Tab Groups* you can toggle between light and dark theme. The Shades-of-gray customizations only take effect with the dark theme.

#### • Bookmarked Speed Dial

Bookmarked Speed Dial ([AMO](href="https://addons.mozilla.org/firefox/addon/bookmarked-speeddial)) is an add-on that offers similar functionality to Vivaldi Speed Dial

The file `bookmarked-speed-dial.css` contains a <em>Shades-of-gray</em> theme customization. Copy this file in addition to `userContent.css` into your *chrome<* directory:

`~/.mozilla/firefox/&lt;name-of-your-profile&gt;/chrome/bookmarked-speed-dial.css`

The directory `../app-gadgets/Firefox-Shades-of-gray/bookmarked-speed-dial-images` contains images wich you can choose as '*Default dial image*' and '*Default folder image*' in the add-on options.

### Inkscape

Original colored icons in Inkscape are hard to identify in dark themes. The file `icon.svg` in folder `Inkscape-icons` contains bright icons.
To use them in Inkscape, the file must be stored in this directory:

`~/.config/inkscape/icons/icons.svg`

> **Note:** not all symbols can be customized because Inkscape is partly using standard GTK symbols ([&#x1f41e;](https://bugs.launchpad.net/inkscape/+bug/789804)).

### Syntax Highlighting

Shades-of-gray includes the syntax color scheme Shades-of-pastel for several editors. By using pastel colors on dark background like pastel chalks on a blackboard the Shades-of-pastel scheme provides balanced and easy on eyes contrasts.

<p align="center">
<img src="https://user-images.githubusercontent.com/22373662/52785609-ad0bd580-3058-11e9-99c1-13c802444149.png" width="773px" height="158px"></img></br><i>Shades of pastel: Bash sample in Sublime Text</i>
</p>

#### • Sublime Text

To install the scheme for Sublime-Text change to directory <code>Shades-of-gray/app-gadgets/Syntax-Colors</code>. Copy the contained file <code>Shades-of-pastel.tmTheme</code> to a folder in your Sublime Packages directory:</p>
```
mkdir -p $HOME/.config/sublime-text-3/Packages/Shades-of-pastel
cp Shades-of-pastel.tmTheme $HOME/.config/sublime-text-3/Packages/Shades-of-pastel/
```
Now you can select Shades-of-pastel as a color scheme in menu *Preferences*.

#### • Gedit, Pluma, Xed, Mousepad

Shades-of-pastel can be used by all editors with syntax highlighting based on *GtkSourceView 3*. To install the color scheme change to directory `Shades-of-gray/app-gadgets/Syntax-Colors`. Copy the contained file `shades-of-pastel.xml` into the following user directory:
```
mkdir -p $HOME/.local/share/gtksourceview-3.0/styles
cp shades-of-pastel.xml $HOME/.local/share/gtksourceview-3.0/styles/
```
Shades-of-pastel is now available in the settings of your editor.

## Requirements

* GTK+ 3.20 or above
* Pixmap theme engine
* Murrine theme engine

## License:

GNU General Public License v3.0

## Screenshots

Cinnamon Patina, Gnome Gray,</br>
Openbox Arch, Xfce4 Cerulean
<p align="center">
<img src="https://user-images.githubusercontent.com/22373662/52785526-8057be00-3058-11e9-8b1f-fa75701b3d1d.jpg" width="45%"></img>  <img src="https://user-images.githubusercontent.com/22373662/52785560-91083400-3058-11e9-93d0-f9fbae247833.jpg" width="45%"></img>  <img src="https://user-images.githubusercontent.com/22373662/52785587-9e252300-3058-11e9-8231-34429b392dbf.jpg" width="45%"></img>  <img src="https://user-images.githubusercontent.com/22373662/52785477-628a5900-3058-11e9-803f-9c75bc6535b0.jpg" width="45%"></img>
</p>
