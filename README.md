#Raw Steps (Still needs LOTS of refinement) 

1. Disable csrutil
1. Install Xcode Command Line Tools
1. Patch RGB Display
1. Install Homebrew
1. Enable csrutil
1. Install homebrew cask
1. Add Brew taps
2. Brew cask packages
  1.Change caffeine icon to retina  
1. Sync Google Chrome
1. Configure Google Chrome extensions
1. Disable spotlight Command Space key to avoid conflicts with alfred
1. Install node packages
1. Set zsh as default - chsh -s $(which zsh) 

1. Install apps via Mac App Store (US)
  1. Coffitivity
  2. iMovie
  3. iPhoto
  4. Keynote
  5. Numbers
  6. Pages
  7. Pocket
  8. Twitter
  9. Xcode

1. Agree to xcode terms command line
1. Install brew packages 
1. npm -g install npm
1. Install node packages 
1. Link apps to their respective folder
  1. Keyboard Maestro
  2. Alfred
  3. aText

1. Remove applications from login
1. If on macbook air, symlink dotfile folder to .dotfiles in home  
1. Install powerline fonts

brew phantomjs required?

1. Enable accessibility for alfred 2, atext, bettertouchtool, dash, chrome, karabiner, keyboard maestro, skype, slate

# OSX Settings

# Icon size of Dock items
defaults write com.apple.dock tilesize -int 43

# Dock magnification
defaults write com.apple.dock magnification -bool true

# Icon size of magnified Dock items
defaults write com.apple.dock largesize -int 52

# Zoom: Options… > Use scroll wheel with modifier keys to zoom: on
defaults write com.apple.universalaccess 'closeViewScrollWheelToggle' -bool true

# Zoom: Options… > Use scroll wheel with modifier keys to zoom: ^ [control]
defaults write com.apple.universalaccess 'HIDScrollZoomModifierMask' -int 262144

# Zoom: Options… > Use keyboard shortcuts to zoom: on
defaults write com.apple.universalaccess 'closeViewHotkeysEnabled' -bool true

#To show removable media (cards, etc):
defaults write com.apple.finder ShowRemovableMediaOnDesktop -bool false

#To show external hard drives (USB, Thunderbolt, firewire, etc):
defaults write com.apple.finder ShowExternalHardDrivesOnDesktop -bool false

#To show mounted servers (AFP, SMB, NFS, etc):
defaults write com.apple.finder ShowMountedServersOnDesktop -bool false

#To show internal hard drives:
defaults write com.apple.finder ShowHardDrivesOnDesktop -bool false

# Set Default keyboard layout
defaults write com.apple.HIToolbox AppleEnabledInputSources -array-add '<dict><key>InputSourceKind</key><string>Keyboard Layout</string><key>KeyboardLayout ID</key><integer>15000</integer><key>KeyboardLayout Name</key><string>USInternational-PC</string></dict>'

# Menu bar: show battery percentage
defaults write com.apple.menuextra.battery ShowPercent -string "YES"

### Spotlight menu keyboard shortcut: none
	/usr/libexec/PlistBuddy "$HOME/Library/Preferences/com.apple.symbolichotkeys.plist" -c 'Delete AppleSymbolicHotKeys:64' > /dev/null 2>&1
	/usr/libexec/PlistBuddy "$HOME/Library/Preferences/com.apple.symbolichotkeys.plist" -c 'Add AppleSymbolicHotKeys:64:enabled bool false'

	### Spotlight window keyboard shortcut: none
	/usr/libexec/PlistBuddy "$HOME/Library/Preferences/com.apple.symbolichotkeys.plist" -c 'Delete AppleSymbolicHotKeys:65' > /dev/null 2>&1
	/usr/libexec/PlistBuddy "$HOME/Library/Preferences/com.apple.symbolichotkeys.plist" -c 'Add AppleSymbolicHotKeys:65:enabled bool false'
	
#disable guest access???????
