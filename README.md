# File: $HOME/.screenrc
hardstatus on
hardstatus alwayslastline
hardstatus string "%{.bW}%-w%{.rW}%n %t%{-}%+w %=%{..G} %H %{..Y} %m/%d %C%a "
###    Keybindings    ##
#
## bind <F7> to detach screen from this terminal
## bind <F8> to kill current session
## bind <F10> to create a new screen
## bind <F9> to rename an existing window
## bind <F11> to move to previous window
## bind <F12> to move to next window
bindkey -k k7 detach
bindkey -k k8 kill
# space in keyboard
bindkey -k k; screen
bindkey -k k9 title
bindkey -k F1 prev
bindkey -k F2 next
displays
multiuser off
hardstatus string "%{.kG}%-Lw%{.KW}%n%f %t%{-}%+Lw %=%{..G} %H %{..W} %d/%m %C%a "
#Start screen windows with blank title
shelltitle ""
# name tiltle window on F1
bindkey -k k1 title
bindkey -k k2 windowlist


## # How to use
#=> AND your are ready to use ! Just type screen on $ prompt !
#=> My config file has following key mapping:
#F1   -  Set a particulate window title e.g. server101
#F2   - Show list of all 40 windows I have open
#F8  - Kill a window  (Message : window number 34 killed)
#F10 - Create new window to run something on this system or open a ssh session to another system
#F11 - Go to just previous windows
#F12 - Go to Just next window
#Cntr-a Ctrl-a - Toggle between 2 windows
#Cntrl-d : Detach screen session. It will keep all your session live. Leave office and go home !
