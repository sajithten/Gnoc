## While entering into exclusive configuration mode by using the " configure exclusive " command, the switch reports the " error: configuration database modified " error and does not allow any configuration.
```
show system users
```
## Login as root user
```
start shell user root
```
## From the shell, issue the mgd clr-chg command.
```
root@jtac-qfx5100-48t-6q-r2284:RE:0% mgd clr-chg                                                                                                                   
root@jtac-qfx5100-48t-6q-r2284:RE:0%
```
## Log in as the intended user and perform configuration by using " configure exclusive ".
