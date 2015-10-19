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
1. Configure powerline font on iterm 
1. Install source code pro

1. Install popcorntime
1. Change permission to allow instalation of apps from anywhere 
1. Wallpaper folder, 30 min, random
1. screensave sliding panel, shuffle order, 20 minutes, show with clock 
1. Create 3 desktops(4 total) with wallpapers on them 
1. Install atom packages from file "apm install --packages-file atom"
1. Gem install bundler
1. bundle install system wide 
1. generate ssh key ssh-keygen -t rsa -b 4096 -C "your_email@example.com" and authorize on github 

1. Set wallpaper folder
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

# Enable tap to click (Trackpad) for this user and for the login screen
defaults write com.apple.driver.AppleBluetoothMultitouch.trackpad Clicking -bool true
defaults -currentHost write NSGlobalDomain com.apple.mouse.tapBehavior -int 1
defaults write NSGlobalDomain com.apple.mouse.tapBehavior -int 1

#Autohide dock
defaults write com.apple.Dock autohide -bool true

#Disable auto correction
defaults write -g NSAutomaticSpellingCorrectionEnabled -bool false
	
#Disable interface sound effects
defaults write com.apple.systemsound "com.apple.sound.uiaudio.enabled" -int 0

# Don’t automatically rearrange Spaces based on most recent use
defaults write com.apple.dock mru-spaces -bool false

# Bottom right screen corner → Start Screen Saver
defaults write com.apple.dock wvous-br-corner -int 5
defaults write com.apple.dock wvous-br-modifier -int 0

# Set preferred language order
defaults write -g AppleLanguages -array "en-US" en

#Currency
defaults write NSGlobalDomain AppleLocale -string "en_US@currency=BRL"
defaults write NSGlobalDomain AppleMeasurementUnits -string "Centimeters"
defaults write NSGlobalDomain AppleMetricUnits -bool true

# Require password immediately after sleep or screen saver begins
defaults write com.apple.screensaver askForPassword -int 1
defaults write com.apple.screensaver askForPasswordDelay -int 0

#Allow apps downloaded from anywhere
sudo defaults write /Library/Preferences/com.apple.security GKAutoRearm -bool NO

# Don't show mirroring options in the menu bar when available
defaults write com.apple.airplay showInMenuBarIfPresent -bool false

#disable guest access???????
