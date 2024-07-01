# Linux Command
Here is a collection of commonly used Linux administration commands across various categories such as user and group management, file system management, process management, networking, and more. These commands are essential for system administrators to manage Linux systems effectively.
## User and Group Management

### Add a New User

```

sudo useradd username

```

```
sudo passwd username

```
### Add a New Group

```
sudo groupadd groupname

```

### Add User to a Group

```
sudo usermod -aG groupname username

```

### Delete a User

```
sudo userdel -r username

```




### Change User Information:

```
sudo chfn username

```

### Change User's Shell

```
sudo chsh -s /bin/bash username

```

## File System Management
### View Disk Usage

```
df -h

```

### View Disk Space Usage by Directory

```
du -sh /path/to/directory

```

### Mount a Filesystem

```
sudo mount /dev/sda1 /mnt

```

### Unmount a Filesystem

```
sudo umount /mnt

```

### Check Disk Usage Inodes

```
df -i

```

### Create a New Directory

```
mkdir /path/to/directory

```

### Change File/Directory Ownership

```
sudo chown user:group /path/to/file_or_directory

```

### Change File/Directory Permissions

```
chmod 755 /path/to/file_or_directory

```

## Process Management
### List Running Processes

```
ps aux

```

### Display System Processes in Real-Time

```
top

```

### Terminate a Process by PID

```
kill PID

```

### Terminate a Process by Name

```
pkill processname

```

### Display Detailed Information about a Process

```
ps -ef | grep processname

```

## Service Management (systemd)
### Start a Service

```
sudo systemctl start service-name

```

### Stop a Service

```
sudo systemctl stop service-name

```

### Restart a Service

```
sudo systemctl restart service-name

```

### Enable a Service to Start at Boot

```
sudo systemctl enable service-name

```

### Disable a Service from Starting at Boot

```
sudo systemctl disable service-name

```

### Check the Status of a Service

```
sudo systemctl status service-name

```

## Networking
### View Network Configuration:

```
ip addr show

```

## View Network Interfaces

```
ifconfig

```

## Check Connectivity with Ping

```
ping google.com

```

## Check Open Ports

```
netstat -tuln

```

## Traceroute to Diagnose Network Issues:

```
traceroute google.com

```
## Check DNS Resolution:

```
nslookup google.com

```

## Security
### Generate SSH Key Pair

```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

```

### Copy SSH Key to Remote Host:

```
ssh-copy-id user@remote_host

```

### Set Up Firewall Rules with UFW:

```

sudo ufw enable

sudo ufw allow 22/tcp

sudo ufw deny 80/tcp

sudo ufw status

```

### Check for Open Ports Using Nmap:

```

sudo nmap -sT localhost

```
Secure Copy Files Between Hosts:

```

scp /path/to/local/file user@remote_host:/path/to/remote/file

```


## System Monitoring

### Monitor System Load:

```

uptime

```


### Check Memory Usage:

```

free -h

```

### Monitor Disk I/O:

```

iostat

```

### View Real-Time System Logs:

```

tail -f /var/log/syslog

```

### Display Kernel Ring Buffer Messages:

```

dmesg

```

### Monitor Network Bandwidth:

```
iftop

```


## Package Management

### Update Package List (Debian-based):



```

sudo apt update

```

### Upgrade All Packages (Debian-based):

```

sudo apt upgrade

```

### Install a Package (Debian-based):


```

sudo apt install package-name

```

### Remove a Package (Debian-based):

```

sudo apt remove package-name

```

### Update Package List (RPM-based):

```

sudo yum check-update

```

### Upgrade All Packages (RPM-based):

```

sudo yum update

```

### Install a Package (RPM-based):

```

sudo yum install package-name

```

### Remove a Package (RPM-based):

```

sudo yum remove package-name

```
