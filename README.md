# ESSENTIAL RECIPES

## Tarball

Decompress:
```bash
$ tar xf [filename]
```
Also, you can install something inside of the tarball:
```bash
$ ./configure
$ make
$ sudo make install
```
###### Note: Example installations;
  * Python
  * Python-pip
  * Node.js

## SSH

### Start sshd service on arch linux
```bash
$ systemctl start sshd.service
```
### File transfer over ssh

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
## Be faster with these tools;

### xclip

```bash
$ sudo apt install xclip
```
To copy ssh public key easily:
```bash
$ xclip -sel clip < ~/.ssh/id_rsa.pub
```
###### See also: 
(Documentation)[https://linux.die.net/man/1/xclip]

## How to uninstall after "make install"
This situation is my most faced one.If you want to get rid of some package that you installed with "make install", follow the lines:

1. Install sudo apt -y install checkinstall

1. cd into source directory that you ran **make install** 
```bash
cd [SOURCE_DIR]
```
2. 

###### See Also: 
(Debian Wiki)[https://wiki.debian.org/CheckInstall], (Homepage)[http://checkinstall.izto.org/index.php]
