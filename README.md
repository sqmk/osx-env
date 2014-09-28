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

## Development stuff

- [Git](http://git-scm.com/download/mac)
- [Packer](http://www.packer.io/downloads.html)
- [Sublime Text](http://www.sublimetext.com/3)
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
