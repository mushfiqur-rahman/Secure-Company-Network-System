### Basic Configuration

### Except host name rest of the command is similar for every switch.

```bash script
en
conf t
hostname MK-SW
line console 0
password cisco login
logging synchronous
exec-timeout 3 0
exit
enable password cisco
banner motd &NO UNAUTHORISED ACCESS!!!&
no ip domain-lookup
service password-encryption
username cisco password cisco
ip domain-name cisco.com
crypto key generate rsa general-keys modulus 1024
ip ssh version 2
line vty 0 15
login local
transport input ssh
exit
access-list 1 permit 192.168.10.0 0.0.0.255
access-list 1 deny any
line vty 0 15
access-class 1 in
exit
do wr
```
