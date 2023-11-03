# KNightAdjuster

Automatically adjust KDE app settings to light or dark mode,
depending on the current [Night Color](https://userbase.kde.org/Tips/Enabling_the_blue_light_filter_on_KDE_Plasma) temperature.

https://github.com/adrium/knightadjuster/assets/23739584/387090b4-f60f-4287-9055-5e01e3367cd4

Supports KDE Plasma, Kate, Konsole, Dolphin, Plasma addons (that follow color schemes),
GTK applications (such as GIMP and LibreOffice), and Google Chrome.

Recommended to use with:

* KDE [Night Color](https://userbase.kde.org/Tips/Enabling_the_blue_light_filter_on_KDE_Plasma)
* Breeze default Plasma Style
* [Circle Clean Window Decoration](https://store.kde.org/p/1997282)
* [Konsole Profiles](https://userbase.kde.org/Konsole#Profile_Management) for light and dark colors

Lightweight alternative to [Yin-Yang](https://github.com/oskarsh/Yin-Yang).

## Configuration

Create the config file `~/.config/knightadjusterrc` to override the following defaults:

	THRESHOLD_DARK=4800

	PLASMA_DARK=BreezeDark
	PLASMA_LIGHT=BreezeClassic
	CURSOR_DARK=Breeze_Snow
	CURSOR_LIGHT=breeze_cursors
	ICON_DARK=breeze-dark
	ICON_LIGHT=breeze
	KONSOLE_DARK=Dark
	KONSOLE_LIGHT=Light
	CHROME_DARK=1
	CHROME_LIGHT=9
	WALLPAPER_DARK=
	WALLPAPER_LIGHT=

## Google Chrome

* Support for [light/dark mode preference](https://github.com/KDE/xdg-desktop-portal-kde/blob/master/src/settings.cpp) since [version 114](https://bugs.chromium.org/p/chromium/issues/detail?id=998903).
* Force dark mode can be set to a value other than 'Default'
  * Enable it here: `chrome://flags/#enable-force-dark`
  * If Chrome is already running, it needs to be restarted to apply the changes
  * The user is prompted to confirm not to interfere with ongoing work
