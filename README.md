# Firewall Checker 
## Windows
### Setup
Enable powershell file execution.
> Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser

### How to use 
Enter command line arguments with comma(`,`)

- first argument : ip addresses 
- second argument : ports
- third argument(optional) : timeout value(default value is 300ms)

```console
PS C:\Users> .\WindowFirewallTest.ps1 "127.0.0.1,192.168.137.1" "32000,139" 500  
=====FIREWALL CHECK START=====
========Timeout : 300ms=======
127.0.0.1 32000 is opened
127.0.0.1 139 is closed
192.168.137.1 32000 is closed
192.168.137.1 139 is opened
=====FIREWALL CHECK END======
```
