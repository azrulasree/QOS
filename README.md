# QOS
Dedicated for learning QOS to optimize bandwidth for certain application in current infrastructure.

Issue:
1) Speed mismatch.
2) Aggregation point.
3) Periodic congestion.

categories QOS:
not strict - best effort
less strict - diffserv ( differentiate services)
strict - IntServ (Integrted services) RSVP - reservation.

QOS Mechanisms:
1) classification and marking
2) Queuing - congestion management. create different queue seperation.
3) congestion avoidance - setting up treshold.
- TCP Slow start -> when TVP flow reduces its window file
- Weighted Random Early Detection (WRED) -> drop random packet when traffic exceed treshold
5) policing and shaping - 
- policing: seting up the rules on packet size. drop if bigger
- shaping -hold packet. change shape if necessary.
6) link efficiency
- compression
- 


setting priority. low priority < high priority
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
