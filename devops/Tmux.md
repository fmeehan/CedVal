# Tmux window multiplexer

https://hackernoon.com/a-gentle-introduction-to-tmux-8d784c404340

## vtop, A graphical activity monitor for the command line

https://github.com/MrRio/vtop

sudo npm install -g vtop

vtop
vtop --theme wizard

## Mac OS X pasteboard

Notes and workarounds for accessing the Mac OS X pasteboard in tmux sessions

[tmux-MacOSX-pasteboard](https://github.com/ChrisJohnsen/tmux-MacOSX-pasteboard)

### Resources 

https://tmuxcheatsheet.com/

## To source .tmux.conf

Inside a tmux session


Prefix+B :
Then type:

source-file ~/.tmux.conf

## To set the theme 

source-file "${HOME}/.tmux-themepack/powerline/block/orange.tmuxtheme"

# Nice tmux themes

[mbdolato](https://github.com/mbadolato/iTerm2-Color-Schemes)

## Better tmux
[Oh my tmux](https://github.com/gpakosz/.tmux)

```
$ cd
$ git clone https://github.com/gpakosz/.tmux.git
$ ln -s -f .tmux/.tmux.conf
$ cp .tmux/.tmux.conf.local .
```