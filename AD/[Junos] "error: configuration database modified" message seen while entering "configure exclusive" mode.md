## While entering into exclusive configuration mode by using the " configure exclusive " command, the switch reports the " error: configuration database modified " error and does not allow any configuration.

Error:
```
root@jtac-qfx5100-48t-6q-r2284>configure exclusive
error: configuration database modified

root@jtac-qfx5100-48t-6q-r2284>
````
Solution:
```
user1@jtac-qfx5100-48t-6q-r2284> show system users
fpc0:
--------------------------------------------------------------------------
4:20AM  up 47 days,  4:09, 1 user, load averages: 0.47, 0.62, 0.61
USER     TTY      FROM                              LOGIN@  IDLE WHAT
user1 p0 100.64.113.16                   4:18AM      - cli
```
# To solve this issue, perform the following steps as the root user:

# Log in as the root user.  
```
root@jtac-qfx5100-48t-6q-r2284> start shell user root
```
# From the shell, issue the mgd clr-chg command.
```
root@jtac-qfx5100-48t-6q-r2284:RE:0% mgd clr-chg                                                                                                                   
root@jtac-qfx5100-48t-6q-r2284:RE:0%
```
# Log in as the intended user and perform configuration by using " configure exclusive ".
```
root@jtac-qfx5100-48t-6q-r2284> configure exclusive                                                                                                                 
warning: uncommitted changes will be discarded on exit                                                                                                             
Entering configuration mode                                                                                                                                                                                    
{master:0}[edit]                                                                                                                                                        
root@jtac-qfx5100-48t-6q-r2284#
```
