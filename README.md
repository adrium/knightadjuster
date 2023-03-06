# KNightAdjuster

Automatically adjust KDE app settings to light or dark mode,
depending on the current [Night Color](https://userbase.kde.org/Tips/Enabling_the_blue_light_filter_on_KDE_Plasma) temperature.

<video src="https://user-images.githubusercontent.com/23739584/223212913-21079f00-c3c0-45f4-8e8c-c71346273f95.mp4" width="480" autoplay loop></video>

Supports KDE Plasma, Kate, Konsole, Dolphin, and Plasma addons that follow color themes.

Recommended to use with:

* KDE [Night Color](https://userbase.kde.org/Tips/Enabling_the_blue_light_filter_on_KDE_Plasma)
* Breeze default Plasma Style
* [Circle Clean Window Decoration](https://store.kde.org/p/1997282)
* [Konsole Profiles](https://userbase.kde.org/Konsole#Profile_Management) for light and dark colors

Lightweight alternative to [Yin-Yang](https://github.com/oskarsh/Yin-Yang).

## Configuration

Create the config file `~/.config/knightadjuster` to override the following defaults:

	THRESHOLD_DARK=4800

	PLASMA_DARK=BreezeDark
	PLASMA_LIGHT=BreezeClassic
	KONSOLE_DARK=Dark
	KONSOLE_LIGHT=Light
