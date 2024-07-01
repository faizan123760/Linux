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
