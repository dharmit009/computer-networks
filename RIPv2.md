# RIPv2

RIPv2 stands for Routing information protocol version 2. RIP in Version 2 can take 16 hops. For configuring rip configuration use router 1841. Add wic-2T module to the router and connect all three routers using serial dce. The dual serial port wic-2T provides higher level of serial port density then a single wan interface card and support speed up to 2.048 mbps. After that give ip addresses and set clock rate to 64000.

RIP Configuration:

* Go to router 0 click on RIP. 
* then go to CLI and run the following: 

``` 
# version 2 
```
* Now go back to gui you will be able to see RIP v2. 
* Add its own router network ID/IP. 
* After that add Your Router 2 network ID/IP.

Do this for all the configuration.d
