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
```sudo usermod -aG groupname username```

### Delete a User
```sudo userdel -r username```

### Change User Information:
```sudo chfn username```

### Change User's Shell
```sudo chsh -s /bin/bash username```

