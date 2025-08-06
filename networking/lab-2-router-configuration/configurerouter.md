In order to Configure the router via CLI, you use the following commands to activeate

- Router> enable
- Router# configure terminal

Once here, you configure the two ports that is connected TO the router ports, NOT the ports connected to the switch ports

To configure LAN1, do the following commands

- Router(config)# interface Gig0/0
- Router(config-if)# ip address 192.168.1.1 255.255.255.0
- Router(config-if)# no shutdown  (even if the port seems on, always run this)
- Router(config-if)# exit

To configure LAN2, do the following commands

- Router(config)# interface Gig0/1
- Router(config-if)# ip address 192.168.2.1 255.255.255.0
- Router(config-if)# no shutdown  (even if the port seems on, always run this)
- Router(config-if)# exit


