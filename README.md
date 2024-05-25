# top-100-linux-commands
Comprehensive list of the top 100 Linux commands with detailed descriptions and usage examples is quite extensive. Below is a subset of this list, showcasing some of the most useful commands for both developers and regular users. Each command includes a description and examples of its usage.

### 1. **ssh**
SSH (Secure Shell) is used to securely connect to a remote machine.
```bash
# Connect to a remote server
ssh username@hostname
# Connect using a specific port
ssh -p 2222 username@hostname
```

### 2. **cd**
Changes the current directory.
```bash
# Change to the home directory
cd ~
# Change to the /etc directory
cd /etc
# Go up one directory level
cd ..
```

### 3. **ls**
Lists directory contents.
```bash
# List files in the current directory
ls
# List all files, including hidden files
ls -a
# List files with detailed information
ls -l
```

### 4. **pwd**
Prints the current working directory.
```bash
pwd
```

### 5. **nano**
Nano is a simple, easy-to-use text editor.
```bash
# Open a file in nano
nano filename.txt
# Save changes and exit
Ctrl + O, Enter, Ctrl + X
```

### 6. **vim**
Vim is a powerful text editor.
```bash
# Open a file in vim
vim filename.txt
# Enter insert mode
i
# Save changes and exit
:wq
```

### 7. **cp**
Copies files and directories.
```bash
# Copy a file
cp source.txt destination.txt
# Copy a directory recursively
cp -r source_dir destination_dir
```

### 8. **mv**
Moves or renames files and directories.
```bash
# Move a file
mv source.txt destination.txt
# Rename a file
mv oldname.txt newname.txt
```

### 9. **rm**
Removes files or directories.
```bash
# Remove a file
rm filename.txt
# Remove a directory and its contents
rm -r directory_name
```

### 10. **chmod**
Changes file permissions.
```bash
# Make a file executable
chmod +x script.sh
# Set specific permissions
chmod 755 filename.txt
```

### 11. **chown**
Changes file owner and group.
```bash
# Change the owner of a file
chown username filename.txt
# Change the owner and group of a directory recursively
chown -R username:group directory_name
```

### 12. **ps**
Displays information about running processes.
```bash
# Display all running processes
ps aux
# Display processes for a specific user
ps -u username
```

### 13. **kill**
Sends a signal to terminate a process.
```bash
# Kill a process by PID
kill 1234
# Force kill a process
kill -9 1234
```

### 14. **top**
Displays real-time system information including processes.
```bash
top
```

### 15. **htop**
An interactive process viewer.
```bash
htop
```

### 16. **df**
Reports disk space usage.
```bash
# Display disk usage in human-readable format
df -h
```

### 17. **du**
Estimates file space usage.
```bash
# Display the size of the current directory and subdirectories
du -h
# Display the size of a specific directory
du -sh directory_name
```

### 18. **tar**
Archives files.
```bash
# Create a tar archive
tar -cvf archive.tar file1 file2
# Extract a tar archive
tar -xvf archive.tar
# Create a gzipped tar archive
tar -czvf archive.tar.gz file1 file2
# Extract a gzipped tar archive
tar -xzvf archive.tar.gz
```

### 19. **gzip**
Compresses files.
```bash
# Compress a file
gzip filename.txt
# Decompress a file
gunzip filename.txt.gz
```

### 20. **find**
Searches for files in a directory hierarchy.
```bash
# Find a file by name
find /path/to/search -name filename.txt
# Find files modified in the last 7 days
find /path/to/search -mtime -7
```

### 21. **grep**
Searches for patterns in files.
```bash
# Search for a pattern in a file
grep 'pattern' filename.txt
# Search recursively in all files in a directory
grep -r 'pattern' /path/to/search
```

### 22. **cat**
Concatenates and displays file content.
```bash
# Display file content
cat filename.txt
# Concatenate multiple files and display the output
cat file1.txt file2.txt
```

### 23. **less**
Views file content one page at a time.
```bash
# View a file
less filename.txt
# Scroll forward and backward
# Forward: Space or f
# Backward: b
```

### 24. **tail**
Displays the last part of a file.
```bash
# Display the last 10 lines of a file
tail filename.txt
# Display the last 50 lines of a file
tail -n 50 filename.txt
# Follow a file (useful for logs)
tail -f filename.txt
```

### 25. **head**
Displays the first part of a file.
```bash
# Display the first 10 lines of a file
head filename.txt
# Display the first 20 lines of a file
head -n 20 filename.txt
```

### 26. **awk**
A powerful text processing language.
```bash
# Print the first column of a file
awk '{print $1}' filename.txt
# Print lines where the second column is greater than 100
awk '$2 > 100' filename.txt
```

### 27. **sed**
A stream editor for filtering and transforming text.
```bash
# Replace 'old' with 'new' in a file
sed 's/old/new/g' filename.txt
# Delete lines containing a pattern
sed '/pattern/d' filename.txt
```

### 28. **scp**
Securely copies files between hosts.
```bash
# Copy a file to a remote host
scp localfile.txt username@remotehost:/path/to/remote/directory
# Copy a file from a remote host
scp username@remotehost:/path/to/remotefile.txt localfile.txt
```

### 29. **rsync**
A fast and versatile file copying tool.
```bash
# Synchronize a local directory with a remote directory
rsync -avz /path/to/local/directory username@remotehost:/path/to/remote/directory
# Synchronize a remote directory with a local directory
rsync -avz username@remotehost:/path/to/remote/directory /path/to/local/directory
```

### 30. **wget**
A non-interactive network downloader.
```bash
# Download a file from a URL
wget http://example.com/file.zip
# Download a file and save it with a different name
wget -O newfile.zip http://example.com/file.zip
```

### 31. **curl**
A tool for transferring data from or to a server.
```bash
# Download a file from a URL
curl -O http://example.com/file.zip
# Download a file and save it with a different name
curl -o newfile.zip http://example.com/file.zip
```

### 32. **apt-get**
A package handling utility for Debian-based systems.
```bash
# Update the package index
sudo apt-get update
# Install a package
sudo apt-get install package_name
# Remove a package
sudo apt-get remove package_name
```

### 33. **yum**
A package manager for RPM-based distributions.
```bash
# Install a package
sudo yum install package_name
# Remove a package
sudo yum remove package_name
# Update all packages
sudo yum update
```

### 34. **pip**
A package manager for Python packages.
```bash
# Install a package
pip install package_name
# Uninstall a package
pip uninstall package_name
# List installed packages
pip list
```

### 35. **docker**
A platform for developing,

 shipping, and running applications in containers.
```bash
# Pull an image from the Docker repository
docker pull image_name
# Run a container from an image
docker run image_name
# List running containers
docker ps
# Stop a running container
docker stop container_id
```

### 36. **systemctl**
Controls the systemd system and service manager.
```bash
# Start a service
sudo systemctl start service_name
# Stop a service
sudo systemctl stop service_name
# Enable a service to start at boot
sudo systemctl enable service_name
# Disable a service from starting at boot
sudo systemctl disable service_name
# Check the status of a service
sudo systemctl status service_name
```

### 37. **journalctl**
Queries and displays logs from journald.
```bash
# View all logs
sudo journalctl
# View logs for a specific service
sudo journalctl -u service_name
# Follow new log entries
sudo journalctl -f
```

### 38. **netstat**
Prints network connections, routing tables, interface statistics, masquerade connections, and multicast memberships.
```bash
# Display all network connections
netstat -a
# Display listening ports
netstat -l
# Display network statistics
netstat -s
```

### 39. **ss**
Utility to investigate sockets.
```bash
# Display all open TCP connections
ss -t
# Display all open UDP connections
ss -u
# Display listening sockets
ss -l
```

### 40. **ifconfig**
Configures network interfaces.
```bash
# Display network interface information
ifconfig
# Assign an IP address to an interface
sudo ifconfig eth0 192.168.1.100
```

### 41. **ip**
Shows/manipulates routing, devices, policy routing, and tunnels.
```bash
# Display network interfaces
ip a
# Assign an IP address to an interface
sudo ip addr add 192.168.1.100/24 dev eth0
# Display routing table
ip route
```

### 42. **ping**
Sends ICMP ECHO_REQUEST packets to network hosts.
```bash
# Ping a host
ping hostname
# Ping a host with a specified number of packets
ping -c 4 hostname
```

### 43. **traceroute**
Prints the route packets take to the network host.
```bash
# Trace the route to a host
traceroute hostname
```

### 44. **nslookup**
Queries the Domain Name System (DNS) to obtain domain name or IP address mapping.
```bash
# Look up the IP address of a domain
nslookup domain.com
```

### 45. **dig**
DNS lookup utility.
```bash
# Perform a DNS lookup
dig domain.com
# Perform a reverse DNS lookup
dig -x ip_address
```

### 46. **hostname**
Shows or sets the system's hostname.
```bash
# Display the hostname
hostname
# Set a new hostname
sudo hostname new_hostname
```

### 47. **whoami**
Displays the current username.
```bash
whoami
```

### 48. **sudo**
Executes a command as another user, typically the superuser.
```bash
# Run a command as the superuser
sudo command
# Edit a file with superuser privileges using nano
sudo nano filename.txt
```

### 49. **passwd**
Changes a user's password.
```bash
# Change your own password
passwd
# Change another user's password (superuser only)
sudo passwd username
```

### 50. **adduser**
Adds a user to the system.
```bash
# Add a new user
sudo adduser username
```

### 51. **usermod**
Modifies a user account.
```bash
# Add a user to a group
sudo usermod -aG groupname username
```

### 52. **deluser**
Removes a user from the system.
```bash
# Remove a user
sudo deluser username
```

### 53. **groupadd**
Adds a new group.
```bash
# Add a new group
sudo groupadd groupname
```

### 54. **groupdel**
Deletes a group.
```bash
# Delete a group
sudo groupdel groupname
```

### 55. **crontab**
Schedules periodic jobs.
```bash
# Edit the current user's crontab
crontab -e
# List the current user's scheduled jobs
crontab -l
```

### 56. **at**
Schedules a command to run at a specific time.
```bash
# Schedule a command to run at a specific time
echo "command" | at 10:00
```

### 57. **uptime**
Shows how long the system has been running.
```bash
uptime
```

### 58. **free**
Displays memory usage.
```bash
# Display memory usage in human-readable format
free -h
```

### 59. **vmstat**
Reports virtual memory statistics.
```bash
# Display virtual memory statistics
vmstat
```

### 60. **iostat**
Reports CPU and I/O statistics.
```bash
# Display CPU and I/O statistics
iostat
```

### 61. **dmesg**
Prints kernel ring buffer messages.
```bash
# Display all messages
dmesg
# Display messages and follow new ones
dmesg -w
```

### 62. **lsblk**
Lists information about block devices.
```bash
# Display block devices
lsblk
```

### 63. **blkid**
Locates and prints block device attributes.
```bash
# Display block device attributes
blkid
```

### 64. **mount**
Mounts a filesystem.
```bash
# Mount a filesystem
sudo mount /dev/sdX1 /mnt
```

### 65. **umount**
Unmounts a filesystem.
```bash
# Unmount a filesystem
sudo umount /mnt
```

### 66. **fdisk**
Manipulates disk partition table.
```bash
# View and edit disk partitions
sudo fdisk /dev/sdX
```

### 67. **mkfs**
Builds a Linux filesystem.
```bash
# Create an ext4 filesystem
sudo mkfs.ext4 /dev/sdX1
```

### 68. **fsck**
Checks and repairs a Linux filesystem.
```bash
# Check and repair a filesystem
sudo fsck /dev/sdX1
```

### 69. **dd**
Converts and copies a file.
```bash
# Create a bootable USB drive
sudo dd if=path/to/image.iso of=/dev/sdX bs=4M status=progress
```

### 70. **parted**
A partition manipulation program.
```bash
# Start parted on a disk
sudo parted /dev/sdX
```

### 71. **rsyslog**
Provides fast, secure, and scalable system logging.
```bash
# Restart rsyslog service
sudo systemctl restart rsyslog
```

### 72. **logrotate**
Rotates, compresses, and mails system logs.
```bash
# Manually rotate logs
sudo logrotate /etc/logrotate.conf
```

### 73. **hostnamectl**
Controls the system hostname.
```bash
# Set the system hostname
sudo hostnamectl set-hostname new_hostname
```

### 74. **timedatectl**
Controls system time and date.
```bash
# Display current time settings
timedatectl
# Set the system timezone
sudo timedatectl set-timezone America/New_York
```

### 75. **hwclock**
Accesses the hardware clock.
```bash
# Display the current hardware clock time
sudo hwclock
# Set the hardware clock to the current system time
sudo hwclock --systohc
```

### 76. **date**
Displays or sets the system date and time.
```bash
# Display the current date and time
date


# Set the date and time
sudo date MMDDhhmmYYYY
```

### 77. **bc**
An arbitrary precision calculator language.
```bash
# Start bc interactive calculator
bc
```

### 78. **expr**
Evaluates expressions.
```bash
# Perform arithmetic operations
expr 2 + 2
```

### 79. **xargs**
Builds and executes command lines from standard input.
```bash
# Use with find to delete files
find /path/to/search -name "*.tmp" | xargs rm
```

### 80. **alias**
Creates an alias for a command.
```bash
# Create an alias
alias ll='ls -la'
# Remove an alias
unalias ll
```

### 81. **echo**
Displays a line of text.
```bash
# Print a string
echo "Hello, World!"
# Print the value of a variable
echo $HOME
```

### 82. **env**
Displays or modifies the environment.
```bash
# Display all environment variables
env
# Run a command with modified environment variables
env VAR=value command
```

### 83. **export**
Sets environment variables.
```bash
# Set an environment variable
export VAR=value
# Export a variable to the environment
export PATH=$PATH:/new/path
```

### 84. **source**
Executes commands from a file in the current shell.
```bash
# Source a script
source script.sh
```

### 85. **history**
Displays the command history.
```bash
# Display command history
history
# Clear command history
history -c
```

### 86. **alias**
Creates an alias for a command.
```bash
# Create an alias
alias ll='ls -la'
# Remove an alias
unalias ll
```

### 87. **man**
Displays the manual for a command.
```bash
# Display the manual for ls
man ls
```

### 88. **info**
Displays the information about commands.
```bash
# Display the info for ls
info ls
```

### 89. **whatis**
Displays a one-line description of a command.
```bash
# Display a one-line description of ls
whatis ls
```

### 90. **apropos**
Searches the manual pages for a keyword.
```bash
# Search for a keyword in the manual pages
apropos keyword
```

### 91. **whereis**
Locates the binary, source, and manual page files for a command.
```bash
# Locate the files for ls
whereis ls
```

### 92. **which**
Locates the executable file associated with a command.
```bash
# Locate the executable for ls
which ls
```

### 93. **type**
Describes a command.
```bash
# Describe the ls command
type ls
```

### 94. **sh**
Executes commands in the Bourne shell.
```bash
# Run a shell script
sh script.sh
```

### 95. **bash**
Executes commands in the Bourne-again shell.
```bash
# Run a shell script
bash script.sh
```

### 96. **zsh**
Executes commands in the Z shell.
```bash
# Run a shell script
zsh script.sh
```

### 97. **ksh**
Executes commands in the Korn shell.
```bash
# Run a shell script
ksh script.sh
```

### 98. **dash**
Executes commands in the Debian Almquist shell.
```bash
# Run a shell script
dash script.sh
```

### 99. **screen**
A terminal multiplexer.
```bash
# Start a new screen session
screen
# Reattach to a detached screen session
screen -r
```

### 100. **tmux**
A terminal multiplexer.
```bash
# Start a new tmux session
tmux
# Reattach to a detached tmux session
tmux attach
```
