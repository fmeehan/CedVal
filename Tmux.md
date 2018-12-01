# Tmux window multiplexer

https://hackernoon.com/a-gentle-introduction-to-tmux-8d784c404340

## Very nice themes

## Install NPM2
sudo npm install pm2@latest -g

http://pm2.keymetrics.io/docs/usage/quick-start/

Target path
/etc/systemd/system/pm2-fmeehan.service
Command list
[ 'systemctl enable pm2-fmeehan' ]
[PM2] Writing init configuration in /etc/systemd/system/pm2-fmeehan.service
[PM2] Making script booting at startup...
[PM2] [-] Executing: systemctl enable pm2-fmeehan...
Created symlink /etc/systemd/system/multi-user.target.wants/pm2-fmeehan.service → /etc/systemd/system/pm2-fmeehan.service.
[PM2] [v] Command successfully executed.


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

## Test Conky

https://www.makeuseof.com/tag/make-linux-system-sexy-conky/

In Iterm2 SSH to a serveur. Start Tmux

Display tmux sessions
tmux new -s myname

petrus ➜  github  tmux ls
1: 1 windows (created Sat Nov 24 13:00:16 2018) [134x62]
fm001: 1 windows (created Fri Nov 23 22:33:58 2018) [184x19]

tmux kill-session -t 1

tmux a -t fm001

Create 3 panes

Cntrl-b + c #trois fois
Cntrl-b + " #to split pane horizontaly

Cntrl-b + w  #Select window to use

Cntrl-b + d  #To disconnect the tmux session

## To source .tmux.conf

Prefix+B :
Then type:

source-file ~/.tmux.conf

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