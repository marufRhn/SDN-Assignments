# SDN-Assignments
1) Write a ryu controller code such that it prints ARP header information by the switch after h1 pings h2.
   Print 1.) ARP source & destination MAC 2.) ARP source & destination IP
2) Write a ryu controller code that create a L2 firewall such that h1 should not be allowed to ping h3 (block MAC Address). Rest of the hosts should be allowed to ping each other.
3) Write a ryu controller code that create a L4 firewall such that communication is not available on a certain port.
   For ex. if port 51000 is blocked then if h1 tries to send tcp traffic to h3 on port 51000 then, it should not be allowed. But if h1 tries to send tcp traffic to h2 on 5500 it should be allowed.
4) Write a ryu controller code that create an IP local balancer such that when h4 send tcp traffic to h5 then it will send traffic equally to h1, h2, h3 in round robin manner.
5) Write a a topology with 4 host such that 2 host are on one VLAN id(VLAN id:-100), while the other 2 hosts are on another VLAN id(VLAN id:-200).
   Then if h1 tries to ping h3 or h4 it will not be allowed, same goes for h2. But h1 can ping h2 and h3 can ping h4.
6) Write a ryu controller code that implements openflow v1.3 and creates two level firewall using two tables where first table will block a packet by source ip and the second table will block the packet by TCP port.
   h1-->h2 (block by IP)
   h3-->h4 (block by TCP port)
   h5-->h6 (ping each other)
