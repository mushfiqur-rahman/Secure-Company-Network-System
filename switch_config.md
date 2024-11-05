### Basic Configuration

```bash script
Switch(config)#
Switch(config)#host
Switch(config)#hostname SM-SW
SM-SW(config)#lin
SM-SW(config)#line cons
SM-SW(config)#line console 0
SM-SW(config-line)#pass
SM-SW(config-line)#password cisco
SM-SW(config-line)#login
SM-SW(config-line)#ex
SM-SW(config-line)#exa
SM-SW(config-line)#exe
SM-SW(config-line)#exec-timeout 3 0
SM-SW(config-line)#logg
SM-SW(config-line)#logging sy
SM-SW(config-line)#logging synchronous
SM-SW(config-line)#ex
SM-SW(config-line)#exi
SM-SW(config-line)#exit
SM-SW(config)#ena
SM-SW(config)#enable pa
SM-SW(config)#enable password cisco
SM-SW(config)#ban
SM-SW(config)#banner mo
SM-SW(config)#banner motd &NO UNAUTHORISED ACCESS!!!&
SM-SW(config)#no ip do
SM-SW(config)#no ip domain-loo
SM-SW(config)#no ip domain-lookup
SM-SW(config)#pass
SM-SW(config)#password ser
SM-SW(config)#ser
SM-SW(config)#service pass
SM-SW(config)#service password-encryption
SM-SW(config)#user
SM-SW(config)#username cisco pas
SM-SW(config)#username cisco password ciso
SM-SW(config)#ip dom
SM-SW(config)#ip domain
SM-SW(config)#ip domain-name cisco.com
SM-SW(config)#cryp
SM-SW(config)#crypto key gen
SM-SW(config)#crypto key generate rsa gen
SM-SW(config)#crypto key generate rsa general-keys mod
SM-SW(config)#crypto key generate rsa general-keys modulus 1024
The name for the keys will be: SM-SW.cisco.com

% The key modulus size is 1024 bits
% Generating 1024 bit RSA keys, keys will be non-exportable...[OK]
*Mar 1 10:49:5.65: %SSH-5-ENABLED: SSH 1.99 has been enabled
SM-SW(config)#ip ssh ver
SM-SW(config)#ip ssh version 2
SM-SW(config)#line vty 0 15
SM-SW(config-line)#login local
SM-SW(config-line)#transport in
SM-SW(config-line)#transport input ssh
SM-SW(config-line)#exit
SM-SW(config)#do wr
Building configuration...
[OK]
SM-SW(config)#
SM-SW#
%SYS-5-CONFIG_I: Configured from console by console

SM-SW#
```
