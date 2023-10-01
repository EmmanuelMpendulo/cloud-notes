### Bash History
	- run last command in history: !ping
	- see last command in history: !ping:p
	- search command prev ran: ctrl + R
	- leave search ctrl + G
	- delete command: hsistory -d <line_number>
	- history - c: delete all history

### Run command without leaving a trace
	- type a space infront of the command
	- you can set HISTCONTROL variable to hide: HISTCONTROL=ingoreboth
	- settings will be lost after system reboot
	- echo "HISTCONTROL=ignoreboth" >> .bashrc
### Record Date and Time for each line in history
	- HISTTIMEFORMAT="%d/%m/%y %T": to set format
	- echo $HISTTIMEFORMAT="%d/%m/%y %T" >> .bashrc: to save the variable in bashrc file

### root vs non-privileged users. Getting root access
	- running a command as root (only users that belong to sudo group [Ubuntu] or wheel [CentOS]): sudo command
	- becoming root temporarily in the terminal: sudo su # => enter the user's password
	-  setting the root password: sudo passwd root
	-  changing a user's password: passwd username
	-  becoming root temporarily in the terminal: su     # => enter the root password

### Find
	- find path -criteria filename : find /etc/ -name passwd
	- case insensive: iname 
	- find /etc/ -name passwd -ls: to execute list for find
	- 