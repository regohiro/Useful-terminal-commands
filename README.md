# Useful-terminal-commands

Allow apps downloaded from anywhere:
sudo spctl --master-disable
sudo spctl --master-enable (set back to default)

Disable opening recent files: 
defaults write com.apple.<App Name> NSQuitAlwaysKeepsWindows -bool false

Disable auto-switching desktops:
defaults write com.apple.dock workspaces-auto-swoosh -bool NO
after, write this:
killall Dock

Disable itunes when play is pressed:
launchctl unload -w /System/Library/LaunchAgents/com.apple.rcd.plist
undo:
launchctl load -w /System/Library/LaunchAgents/com.apple.rcd.plist
