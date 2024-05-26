# TMUX config file and basic navigation notes

Feel free to use/share my config file and general notes

Cheers


PREFIX= ctrl + b 
ctrl + b = to create command for tmux

DETACH FROM SESSION= ctrl + 'b' then 'd' (session still live just detached)

LIST ACTIVE SESSIONS = tmux list-sessions or tmux ls

REATTACH TO SESSION = tmux attach or tmux a

KILL TMUX Server, discconect from all tmux sessions = tmux kill-server && tmux

**DEFAULT NON CONFIGURED TMUX COMMANDS**:

SPLIT SCREEN VERTICAL = prefix then shift + 5 (repeat to do again)

SPLIT SCREEN HORIZONTAL = prefix then shift + double quote " 

NAVIGATE TO ANOTHER PANE/QUADRANT AFTER SPLIT = prefix + control arrow

exit pane = exit (if you exit out of all you are no longer) connected 
exit without having to tyrpe anything = prefix + x (in the selected pane)

**WINDOWS MANAGEMENT:**

CREATE NEW WINDOWS IN TMUX = tmux new-window  
W/O typing command = prefix + c

SWITCH BETWEEN WINDOWS = prefix + p (previos) or prefix +n (next)

TO KILL A WINDOW = prefix + &

prefix + ~ show messages -basically shows some history of what was typed, discovered by accident-- Hit EXIT to exit

REMANE A WINDOW = (make sure you are on that window) prefix + comma 
or tmux rename-window 


**SESSION/WINDOW MANAGEMENT:**

list sessions command while in TMUX will show you how many sessions plus the one you're attached to

REATTACH = tmux attach (will attach you to session most recently used)

ATTACH TO SPECIFIC WINDOW = Exit out of tmux (possible nesting issues if you dont) and tmux a -t + session number (ex.0,1,2) or name (if you renamd it)

ATTACH TO A SPECIFIC WINDOW W/O EXIT = prefix + s select session using arrows then enter

RENAME A SESSION while attached to session = tmux rename-session whatevername
or prefix $

RENAME A WINDOW IN THAT SESSION = tmux rename-window -t + window number(0,1,2 etc) whatever name

**CONFIG NAVIGATION SETTINGS:**

RELOAD TMUX CONFIG FILE W/O EXIT TMUX = prefix + r 

SPLIT SCREEN = prefix + v  (vertical)  prefix + z (horizontal)

NAVIGATE TO DIFFERENT PANES = alt + arrows

NAVIGATE TO DIFFERENT WINDOWS = Shift + keyboard arrows

CHANGE WINDOW ORDER = ctrl + shift + keyboard arrows

SYNC PANES ON/OFF = prefix + y  


**GENERAL ITEMS:**

INSTALL TMUX PACKAGE = prefix + I















