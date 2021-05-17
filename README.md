# Configuring-VLANs-and-Trunk

In this project vlans and trunk links are configured on the switches. The topology consists of 3 PCs and 2 Switches. 

The topology of the projects is shown below:
![image](https://user-images.githubusercontent.com/69259617/118564482-55c8a400-b73e-11eb-9999-d00b5063efc6.png)

Firstly, the basic switch configurations are configured such as hostname, line console and vty line passwords, password encryption etc.

To configure VLANs, a very simple command is issued, **vlan 10**. By issuing this command vlan 10 is created. Similarly other vlans are created. Initially, the ip address was assigned to Vlan 1 but then this is moved to vlan 99. This is done for security purpose. Same is done on switch S2. A trunk link is established between the two switches, S1 and S2, and this is a dynamic desirable or DTP trunk link. By default all the vlans are allowed on this trunk link and in this project activity the defaults setting are kept. 

Connectivity tests are condicted in order to see if the system is working. PC-A can ping PC-B because these two PCs are in the same vlan. However, the PCs cannot ping the switches since both the devices are on different networks. 

Conducting connectivity tests for one last time shows that the trunk links and vlans are successfully configured. 
