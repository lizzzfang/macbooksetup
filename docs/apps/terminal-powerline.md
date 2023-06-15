# Terminal + Powerline

[Powerline](https://github.com/powerline/powerline) Powerline is a statusline plugin for vim, 
and provides statuslines and prompts for several other applications, 
including zsh, bash, fish, tmux, IPython, Awesome, i3 and Qtile.

## Prerequisites

Fonts should be installed as described in [Essentials](../essentials/essentials.md#Fonts) section.

## Installation

Install Python3 via homebrew (Optional: in case you do not have pyhton installed. run python3 --version to see if it's installed)
```shell
 brew install python3
```

Install powerline via pip (python package manager)
```shell
 pip3 install powerline-status
```

Find the location
```shell
 pip3 show powerline-status
```
It shows that the powerline-status is installed at /Users/yifeifang/Library/Python/3.9/lib/python/site-packages

## Configuration
To activate powerline, you need to source powerline.sh in your .zshrc

Open up your .zshrc in Vim or any editor
```shell
 vi ~/.zshrc
```

Add bin to PATH and add the daemon with a proper location 
```zsh
# Powerline
export PATH=$PATH:$HOME/Library/Python/3.9/bin
powerline-daemon -q
POWERLINE_BASH_CONTINUATION=1
POWERLINE_BASH_SELECT=1
source /Users/yifeifang/Library/Python/3.9/lib/python/site-packages/powerline/bindings/zsh/powerline.sh
```
## Customization

To add a new theme:

1. Go to http://ethanschoonover.com/solarized
2. Scroll down and download the Theme (solarized.zip)
3. Extract the solarized.zip file
4. Open the osx-terminal.app-colors-solarized folder. This folder contains Theme for the terminal.
5. Double click “Solarized Dark ansi.terminal” file — This is the specific Theme file for Terminal.app. 
Note: If you get a warning that this is from an unidentified developer, Right-click on the file and select “Open with” > Terminal option.
6. At this point, you have the Theme installed into your Terminal. We just need to make it a default Theme.
7. Open Terminal > Preferences > Text and select the “Solarized Dark …” theme and click on “Default”.

## Fonts
After fonts are installed, don't forget to change the font in terminal. Otherwise, powerline won't be displayed properly.
1. Open Terminal > Preferences > Text
2. Select Solarized Dark ansi Theme
3. Click on the “Font” button — This opens up “Fonts” dialog
4. In the “Fonts” dialog, select “Meslo LG L DZ for Powerline” in the Family and also select font size 14 
(so it’s easier to read).

## Reference
[How to Jazz Up Your Bash Terminal](https://www.freecodecamp.org/news/jazz-up-your-bash-terminal-a-step-by-step-guide-with-pictures-80267554cb22/)

[How to install Powerline to pimp your BASH prompt (For Mac)](https://medium.com/@ITZDERR/how-to-install-powerline-to-pimp-your-bash-prompt-for-mac-9b82b03b1c02)
