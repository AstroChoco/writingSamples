# How a GPON network works?
The bandwidth of an optical fiber is divided by several logical traffic containers. Each container consists of a number of logical GEM ports through which the OLT can communicate traffic with the ONT over the optical fiber. The capacity of each container and service traffic that each GEM port carries is determined by the practical network deployment.

## How traffic travels from ISPs to Subscribers?
Downstream traffic from ISPs enters the GPON network through the OLTs and to ONTs toward subscriber premises.

1. The OLTs multiplex downstream traffic and convert the electrical signals to fiber-optic light signals:

   1. The OLTs classify the traffic by previously defined matching rules which may target some or all of the fields of one packet, such as source IP address, destination IP address, source MAC address and destination MAC address.
   
   2. The OLTs tag the traffic with service virtual LAN (VLAN) IDs upon practice.
   
   3. The OLTs route traffic through the optical fiber to the GEM port associated with the MAC address or the VLAN ID by looking up in the previously learned or defined traffic forwarding table.

3. The ONTs demultiplex downstream traffic and convert the fiber-optic light signals to electrical signals: 

   1. The ONTs transform the fiber-optic signals to electrical signals via GEM ports.

   2. The ONTs process tags of traffic.

   3. The ONTs send the traffic to the corresponding interface.
   
## How traffic travels from Subscribers to ISPs?
Upstream traffic from subscribers enters the GPON network through the ONTs and to OLTs toward ISPs.

1. The ONTs convert the electric signals of the upstream traffic to fiber-optic light signals and send them to the OLTs: 

   1. The ONTs send the traffic to the corresponding interface.
   
   2. The ONTs tag the traffic with the VLAN ID associated with the ONT and service VLAN ID.
   
   3. The ONTs route the traffic of a service to the corresponding GEM ports.

2. The OLTs convert the fiber-optic light signals of upstream traffic to electrical signals and aggregate them:

   1. The OLTs transform the fiber-optic signals to electrical signals.
   
   2. The OLTs process tags of traffic including addition of the system VLAN ID.
   
   3. The OLTs aggregate the traffic and sends it to the destination by looking up in the previously learned or defined traffic forwarding table.



