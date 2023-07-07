# LINUX NOTES

### Setup a custom ssh login banner and message of the dat (MOTD)
#### Banner File:
Create the ssh banner file
- sudo vi /etc/ssh/banner_file
- type custom banner and save file
Configure the ssh daemon
- sudo vi /etc/ssh/sshd_config
- find the the line that starts with #Banner and remove the # and add the path of the banner file: #Banner /etc/ssh/banner_file

#### MOTD:
Create MOTD file
- sudo vi /etc/motd
- type in message of the day and save file
- restart the ssh daemon : sudo systemctl restart ssh