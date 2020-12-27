# Automating EVPN VXLAN with BGP Unnumbered

### Automating Cumulus Flat Files

# IMPORTANT NOTE: 
Device R3 and R4 will not learn each others loopbacks. Nor will device R5 and R6 learn each others.
This is because they share the same Autonomous System and have learned that prefix via the Spine. 
This is a BGP loop prevention mechanism and is expected behaviour. If you want to have traffic to pass freely between these devices, change the device autonomous system value for the 4 leafs in the host_vars directory to ensure that all leaf have unique ASNs.
i.e.:

R3: 65003

R4: 65004

R5: 65005

R6: 65006

![alt text](https://github.com/IPvZero/EVPN-VXLAN-Cumulus/blob/main/images/evpn.png?raw=true)

![alt text](https://github.com/IPvZero/EVPN-VXLAN-Cumulus/blob/main/images/evpn4.png?raw=true)


### About Me
My name's John McGovern, I maintain a Youtube channel called IPvZero and I am trainer for CBT Nuggets. 
I create instructional videos on Python Network Automation.

### Contact

[Twitter](https://twitter.com/IPvZero)

[Youtube](https://youtube.com/c/IPvZero)

[LinkedIn](https://www.linkedin.com/in/ipvzero)

### CBT Nuggets 

[Advanced Network Automation with Cisco and Python](http://learn.gg/adv-net)
