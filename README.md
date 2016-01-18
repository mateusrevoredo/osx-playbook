#Raw Steps (Still needs LOTS of refinement) 

1. Disable csrutil
1. Install Xcode Command Line Tools xcode-select --install
1. Patch RGB Display
1. Install Homebrew
1. Enable csrutil
1. Install homebrew cask
1. Add Brew taps
2. Brew cask packages
  1.Change caffeine icon to retina  
1. Sync Google Chrome
1. Configure Google Chrome extensions
1. Install node packages
1. Set zsh as default shell /usr/local/bin/zsh
1. show volume on menubar 
1. download and install windows virtual machines from https://dev.windows.com/en-us/microsoft-edge/tools/vms/mac/ 


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
  10. Telegram
1. Install apps via Mac App Store (BR)
  1. Reeder
  2. DayOne


1. Agree to xcode terms command line
1. Install brew packages 
1. Enable fzf extensions with /usr/local/opt/fzf/install 
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
1. Install vpn software

1. Install popcorntime
1. Change permission to allow instalation of apps from anywhere 
1. Wallpaper folder, 30 min, random
1. screensave sliding panel, shuffle order, 20 minutes, show with clock 
1. Create 3 desktops(4 total) with wallpapers on them 
1. Install atom packages from file "apm install --packages-file atom"
1. Gem install bundler
1. bundle install system wide 
1. generate ssh key ssh-keygen -t rsa -b 4096 -C "your_email@example.com" and authorize on github 
1. set modifier keys caps-lock on both keyboards to none (manually for now)  
1. check all mouse/keyboard gestures (manually for now) 
1. disable icloud sync for photos, mail, keychain, back to my mac
1. set user profile avatar
1. display login window as list of users
1. show fast user switching menu
1. mac app store free downloads save password, purchases after 15 minutes 
1. Install adobe ICC color profiles 
1. Install java for osx https://support.apple.com/kb/DL1572?viewlocale=en_US&locale=en_US 
1. Install meteor curl https://install.meteor.com/ | sh
1. Add vagrant to sudoers to avoid nfs password
Cmnd_Alias VAGRANT_EXPORTS_ADD = /usr/bin/tee -a /etc/exports
Cmnd_Alias VAGRANT_NFSD = /sbin/nfsd restart
Cmnd_Alias VAGRANT_EXPORTS_REMOVE = /usr/bin/sed -E -e /*/ d -ibak /etc/exports
%admin ALL=(root) NOPASSWD: VAGRANT_EXPORTS_ADD, VAGRANT_NFSD, VAGRANT_EXPORTS_REMOVE

1. Install plugin: vagrant plugin install vagrant-vbox-snapshot
2. Install plugin: vagrant plugin install vagrant-hostsupdater

#Macbook air steps
1. If on macbook air, move pictures folder to external hd and symlink to dropbox
1. Move virtualbox default machine folder to external HD 
1. Copy dotfiles folder to local .dotfiles and symlink to dropbox (When pc boots configuration must be there)
1. link vagrant.d to external hd
1. copy wallpaper folder to local .wallpapers and symlink to dropbox (When pc boots configuration must be there)

1. Set wallpaper folder
2. Download https://github.com/JohnCoates/Aerial and set as my screensaver

brew phantomjs required?

1. Enable accessibility for alfred 2, atext, bettertouchtool, dash, chrome, karabiner, keyboard maestro, skype, slate
