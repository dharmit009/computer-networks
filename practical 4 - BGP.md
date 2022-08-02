# Broader Gateway Protocol (BGP):

**What is Broader Gateway Protocol?**

Broader Gateway Protocol (BGP) is an interdomain routing protocol which is used to share routing information between autonoumous devices. 

There are many protocols like rip, arp, and more.
each and each info at each and every hop is maintained 

One entire network is considered as `autonoumous system` this system are given numbers like 100, 200, and further. 

Router0 > CLI > yes > once you have the prompt type > enable > after that the prompt will change to # > then type `config terminal` > router bgp 100 > your prompt will change to `Router(config-router)` > neighbor 10.0.0.2 remote-as 200 > network 10.0.0.0 mask 255.0.0.0 > exit


**STEPS:**

* Click on `Router0`. 
* Go to `CLI` tab & press enter to go into command mode.
* After that type `enable` which will change your router prompt to `Router0#`.
* Now change your router mode to configure terminal by `config terminal` this will change your router mode to `Router0(config-router)#`.
* Now type the following to setup BGP: `neighbor 10.0.0.2 remote-as 200`. Here, 200 is the next given number to the autonomous system.
* Once You have completed that provide the following: `network 10.0.0.0 mask 255.0.0.0` which the current routers and the next routers common network with mask.
