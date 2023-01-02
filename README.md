# QOS
Dedicated for learning QOS to optimize bandwidth for certain application in current infrastructure.

setting priority. low priority < high priority.
reserving bandwidth

understand type of packet that will arrive.
ACL. (ip source ip destination, port source, port destination)

classification and marking. deploy tag
1) IP Precedence  | IP Header (3bits) - 0-7
2) DSCP | IP Header (3bits) - 0-63
3) COS (Class Of Services)
- ETH Header (3bits) 
- user VLAN Tag -> require Trunk | 802.1p
- 3 bits : 0-7 | 6 and 7 are reserve for Network Control Traffic
