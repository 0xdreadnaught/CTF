# Running services

### show running processes

`ps -eF`

### Show running proccesses owned by root

`ps -eF | grep root`


# Running network services

### Listening ports and associated process

`netstat -tlnup | grep LISTEN`

### Listening ports

`netstat -ano | grep LISTEN`

### Listening TCP ports

`netstat -anp tcp | grep LISTEN`

### Listening UDP ports
`netstat -anp udp | grep LISTEN`


# User Enumeration

### Find all user accounts

`cat /etc/passwd`

### Find all user groups

`cat /etc/group`

### Find current user

`whoami`

### Find current user and groups

`id`

### Find groups for specific user

`id <username>`

### Find who is logged in

`who`

# Basic System Information

### Find basic networking info

`ifconfig`

`ip`

### Find ip routing info

`ip route`

### Find ARP records

`arp -a`

### Show current OS distro

`cat /etc/redhat-release`

`cat /etc/os-release`

### Get kernel info

`uname -a`

`uname -srm`

# File information

### Show file type

`file <filename>`

### Show where a command links to

`which <binary>`

### Locate a file or binary

`locate <filename>`

### Find SUID files

`find / -type f -perm 4000 2>/dev/null`

### Find files owned by root
`find / -type f -user root 2>/dev/null`
