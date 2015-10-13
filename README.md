#Raw Steps (Still needs LOTS of refinement) 

1. Disable csrutil
1. Install Xcode Command Line Tools
1. Patch RGB Display
1. Install Homebrew
1. Enable csrutil
1. Install homebrew cask
1. Add Brew taps
1. Sync Google Chrome
1. Configure Google Chrome extensions
1. Install Smooth Mous (check if it has a defaults write)
  1. Mouse 2 - Speed
  2. Trackpad 7 - Speed
1. Link .gauth file
1. Disable spotlight Command Space key to avoid conflicts with alfred
1. Install node packages

1. Install apps via Mac App Store
  1. Coffitivity
  2. iMovie
  3. iPhoto
  4. Keynote
  5. Numbers
  6. Pages
  7. Pocket
  8. Twitter
  9. Xcode


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
