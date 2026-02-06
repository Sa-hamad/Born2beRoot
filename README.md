_This project has been created as part
of the 42 curriculum by **sahamad**_<sahamad>.

# Born2beRoot
Creating a virtual machine in VirtualBox. The goal is to set up an operating system while implementing specific rules.

## Description
_Clearly presents the project, including its goal and a brief overview._

### Born2beRoot
Intro to Server management and working with root access. Setting up and configuring a virtual machine using VirtualBox with Debian.

### Overview
- Setting up encrypted partitions, configuring SSH
- Managing users.
- Writing a monitoring script.
- Set up a virtual machine in VirtualBox with Debian
- Configure encrypted partitions using LVM
- Set up and configure SSH server on a non-standard port
- Configure firewall (UFW for Debian)
- Implement strict password policies and sudo rules
- Create users and groups with specific permissions
- Write a monitoring script that displays system info (architecture, CPU, RAM, disk usage, network info, etc.)
- Set up cron jobs to run the monitoring script automatically every 10 mins.

## Instructions
_Relevant information about compilation, installation, and/or execution._

#### To start VM
- Open VirtualBox and start the VM
- The server will boot up and ask for the encryption password set during installation.
- After decryption, it'll boot into the login screen

#### Logging in
- Can't log in as root directly (disabled for security)
- Log in with regular user account (username & pass)
- Use su to get root privileges

#### Connecting via SSH in a terminal
- From host machine terminal: ssh username@localhost -p 4242.
- it will then ask for the password

## Resources
_Classic references related to the topic (documen- tation, articles, tutorials, etc.), as well as a description of how AI was used — specifying for which tasks and which parts of the project._

**Virtual Machine** 
[https://cloud.google.com/learn/what-is-a-virtual-machine]
[https://wiki.debian.org/LVM]
[https://www.youtube.com/watch?v=dMHFArkANP8&list=PLvrGkX6pcHIC8-UKfChyYGcQtvJtniH3c&index=3]

**Partitions**
[https://www.redhat.com/en/blog/lvm-vs-partitioning]

**Virtualbox / Debian**
[https://www.virtualbox.org/manual/topics/Introduction.html#ct_about-virtualbox]

**Users & Groups**
[https://www.linode.com/docs/guides/linux-users-and-groups/]

**Virtual Box** 
[https://www.virtualbox.org/manual/ch01.html] 

**Firewall**
[https://www.digitalocean.com/community/tutorials/how-to-set-up-a-firewall-with-ufw-on-ubuntu]

**Script**
[https://www.geeksforgeeks.org/linux-unix/introduction-linux-shell-shell-scripting/]
[https://www.geeksforgeeks.org/linux-unix/crontab-in-linux-with-examples/]

Also got helpful tips and advice from other students working on the project. 

### AI Tools
Used AI (Claude, ChatGPT, Gema) used AI to help me understand what was going wrong and tips how to fix it. I also used it to review and understand specific concepts better and commands.

## Notes

### Files
	cat <file>                  # View file
	less <file>                 # View file (scrollable)
	nano <file>                 # Edit file

### Search
	grep "text" <file>          # Search in file
	grep -r "text" /path        # Search in directory
	find . -name "*.txt"        # Find files

### Count
	wc -l <file>                # Count lines
	ls | wc -l                  # Count files

### Pipes
	command | grep "text"       # Filter output
	command > file              # Save to file
	command >> file             # Append to file

### Files
	rm <file>                   # Delete
	rm -l						# Delete a directory with a file
	rm -lf						# Force delete a directory with file
	rmdir						# Delete a directory

### Navigation
	pwd                         # Current directory
	cd <dir>                    # Change directory
	ls -lah                     # List files (detailed)

### Process
	ps aux | grep <name>        # Find process
	kill <PID>                  # Kill process
	top                         # Monitor processes

### System
	df -h                       # Disk space
	free -h                     # Memory usage
	sudo reboot                 # Restart

# Shortcuts
	history                     # Command history
	!!                          # Repeat last command
	Ctrl+R                      # Search history
	Ctrl+C                      # Cancel command
	Ctrl+L                      # Clear screen