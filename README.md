# mikrotik-cheatsheet


### RouterOS version

`system resource print`

### Backup system

`system backup save name=somename`

### Backup configuration

`export file=some_file`

### List existing files

`file print`

### Download backup

Official Mikrotik docs offers to use FTP for downloading files from the device. Since the protocol is old and not secure, we can use SFTP instead:

`scp admin@192.168.88.1:basic.backup basic.backup`

Where `basic.backup` is the filename from `file print`.
