# essential-recipes


## SSH

### Start sshd service on arch linux
```bash
$ systemctl start sshd.service
```
### File transver over ssh

Syntax:

```bash
$ scp <source> <destination>
```

To copy a file from B to A while logged into B:

```bash
$ scp /path/to/file username@a:/path/to/destination
```

To copy a file from B to A while logged into A:

```bash
$ scp username@b:/path/to/file /path/to/destination
```


## Arch Linux

###  Instal aur packages in arch linux:

```bash
$ makepkg -si //clone repository and cd into it than type this command
```



