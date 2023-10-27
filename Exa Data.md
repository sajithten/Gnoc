![image](https://github.com/sajithten/Gnoc/assets/110303586/bb917666-3f1a-467d-9c81-63cdd3ff6513)

Top of rack is the only switch available in the server rack (TOR)
Agg/dist – OOB switch 
Acc – production switches/uplink production switches
Ts (terminal server) – console device and the management (mention the port num)

in dist- search for vlan
show int ethernet1/39-42 status -- int connected status and for VLAN
show int description |include TOR  -- port channel
