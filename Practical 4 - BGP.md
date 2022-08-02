# Broader Gateway Protocol (BGP):

**What is Broader Gateway Protocol?**

Broader Gateway Protocol (BGP) is an interdomain routing protocol which is used to share routing information between autonoumous devices. 

There are many protocols like rip, arp, and more.
each and each info at each and every hop is maintained 

One entire network is considered as `autonoumous system` this system are given numbers like 100, 200, and further. 

Router0 > CLI > yes > once you have the prompt type > enable > after that the prompt will change to # > then type `config terminal` > router bgp 100 > your prompt will change to `Router(config-router)` > neighbor 10.0.0.2 remote-as 200 > network 10.0.0.0 mask 255.0.0.0 > exit


**STEPS:** (DONT FOLLOW THIS STEPS NEED TO REWRITE ...)

* Click on `Router0`. 
* Go to `CLI` tab & press enter to go into command mode.
* After that type `enable` which will change your router prompt to `Router0#`.
* Now change your router mode to configure terminal by `config terminal` this will change your router mode to `Router0(config-router)#`.
* Now type the following to setup BGP: `neighbor 10.0.0.2 remote-as 200`. Here, 200 is the next given number to the autonomous system.
* Once You have completed that provide the following: `network 10.0.0.0 mask 255.0.0.0` which the current routers and the next routers common network with mask.


(Follow this steps instead...)


## Router 0 Config: 
Router(config)#router bgp 100
Router(config-router)#neighbor 30.0.0.2 remote-as 200
Router(config-router)#network 10.0.0.0 mask 255.0.0.0
Router(config-router)#exit
Router(config)#exit
Router#
%SYS-5-CONFIG_I: Configured from console by console
Router#%BGP-5-ADJCHANGE: neighbor 30.0.0.2 Up


## Router 1 config: 

Router(config)#router bgp 200
Router(config-router)#neighbor 30.0.0.1 remote-as 100
Router(config-router)#%BGP-5-ADJCHANGE: neighbor 30.0.0.1 Up
Router(config-router)#neighbor 70.0.0.2 remote-as 3100
Router(config-router)#neighbor 70.0.0.2 remote-as 300
Router(config-router)#network 50.0.0.0 mask 255.0.0.0
Router(config-router)#exit
Router(config)#exit
Router#
Router#exit

## Router 2 Config: 

Router(config)#router bgp 300
Router(config-router)#neighbor 70.0.0.1 remote-as 200
Router(config-router)#%BGP-5-ADJCHANGE: neighbor 70.0.0.1 Up
Router(config-router)#network 90.0.0.0 mask 255.0.0.0
Router(config-router)#exit
Router(config)#exit
Router#
%SYS-5-CONFIG_I: Configured from console by console

