# QOS
Dedicated for learning QOS to optimize bandwidth for certain application in current infrastructure.
To prevent Tail Drop -> where all incoming packet are dropped when memory buffer are full.

Issue:
1) Speed mismatch.
2) Aggregation point.
3) Periodic congestion.
4) Lack of bandwidth
5) Latency(Delay) & Jitter
6) Packet Loss

## categories QOS / QOS Model:
not strict - best effort
|
V
strict - IntServ (Integrted services) RSVP protocol - reserve bandwidth along all network.
|
V
less strict - diffserv ( differentiate services) - tagging/ DSCP marking 

## Method Of Classifying:
![image](https://user-images.githubusercontent.com/83261924/210411436-fc79c8a4-90d3-48e9-827e-618665249d28.png)
COS: Class of Service - layer2
TOS: Types of Service - layer3 (IPP - old / DSCP - new)
Network Based Application Recognition 2 (NBAR) - NBAR Application Files define traits of application(application signature)

## Method of Marking:
![image](https://user-images.githubusercontent.com/83261924/210452009-ca80c520-8f35-4e6e-a0b7-f9b7d7b22086.png)



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
