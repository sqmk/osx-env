# OSX Environment

Listed here are the applications and settings I use for OSX.

## Applications

- [Adobe Flash](http://get.adobe.com/flashplayer/)
- [Dropbox](https://www.dropbox.com/downloading?src=index)
- [Evernote](https://evernote.com/download/)
- Final Cut Pro (Local)
- [Firefox](https://www.mozilla.org/en-US/firefox/new/)
- [Google Chrome](https://www.google.com/chrome/browser/)
- [Pixelmator](https://itunes.apple.com/us/app/pixelmator/id407963104)
- [Skype](http://www.skype.com/en/download-skype/skype-for-computer/)
- [The Unarchiver](https://itunes.apple.com/us/app/the-unarchiver/id425424353)
- [Transmission](https://www.transmissionbt.com/download/)
- Transmit (Local)

## Mouse settings
```ssh
defaults write -g com.apple.swipescrolldirection -bool FALSE
defaults write com.apple.driver.AppleBluetoothMultitouch.mouse MouseButtonMode TwoButton
osascript -e 'tell app "System Events" to log out'
```

## Prevent DS_Store

```ssh
defaults write com.apple.desktopservices DSDontWriteNetworkStores true
```

## Development stuff

- [Docker](https://github.com/boot2docker/osx-installer)
- [Git](http://git-scm.com/download/mac)
- [Packer](http://www.packer.io/downloads.html)
- [Sublime Text](http://www.sublimetext.com/3)
- [Vagrant](https://www.vagrantup.com)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
- [Xcode](https://itunes.apple.com/us/app/xcode/id497799835)

## Git configuration

```ssh
git config --global user.name "Michael K. Squires"
git config --global user.email sqmk@example.com
```

## Packer configuration

```ssh
echo 'export PATH=$PATH:/usr/local/packer' >> ~/.profile
```

## New development sparsebundle

```ssh
mkdir ~/Development
hdiutil create -size 16g -fs 'Case-sensitive HFS+' -type SPARSEBUNDLE -volname Development ~/Development/Development.sparsebundle
```

## Sublime Configuration

- [Sublime Package Manager](https://sublime.wbond.net)
- Abacus
- DocBlockr
- Puppet
- SideBarEnhancements
- SyncedSideBar
- [Theme - Soda](https://github.com/buymeasoda/soda-theme/)
- [Font - Inconsolata](http://levien.com/type/myfonts/inconsolata.html)

### User settings

```json
{
	"auto_complete": true,
	"color_scheme": "Packages/User/Monokai Soda.tmTheme",
	"font_face": "Inconsolata",
	"font_size": 14,
	"highlight_line": true,
	"ignored_packages":
	[
		"Vintage"
	],
	"rulers":
	[
		80,
		120
	],
	"shift_tab_unindent": true,
	"soda_folder_icons": true,
	"theme": "Soda Dark 3.sublime-theme"
}
```

### PHP Settings

```json
{
	"tab_size": 4,
	"translate_tabs_to_spaces": true,
	"ensure_newline_at_eof_on_save": true,
	"trim_trailing_white_space_on_save": true,
	"extensions": ["php"],
	"com.khiltd.abacus.separators": [
		{
			"token": "=>",
			"gravity": "right",
			"preserve_indentation": true
		}
	]
}
```
