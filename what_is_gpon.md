# What is GPON?
Gigabit-capable passive optical network (GPON) is a network architecture developed by ITU-T. GPON uses optical fibers as the physical media to transmit data with a downstream (to subscribers) speed up to 2.5 Gbps and an upstream speed up to 1.25 Gbps (from subscribers). A GPON network is also addressed as the last-mile connection with a service range of 20 km at maximum.

A GPON network consists of the following components:

* __Optical Line Terminations (OLTs)__ multiplex downstream traffic and convert the electrical signals to fiber-optic light signals; convert the fiber-optic light signals of upstream traffic to electrical signals and aggregate them.
  
* __Optical splitters__ split the fiber-optic light signals for them to reach individual premises
  
* __Optical Network Terminations (ONTs)__ demultiplex downstream traffic and convert the fiber-optic light signals to electrical signals; convert the electric signals of the upstream traffic to fiber-optic light signals and send them to the OLT.
  
All of the components are connected to each other through a single optical fiber cable. GPON network uses different wavelengths of light to transmit data in different directions:

* Wavelength of 1490nm transmits downstream voice and data traffic

* Wavelength of 1550nm transmits downstream video traffic

* Wavelength of 1310nm transmits upstream subscriber traffic

## What are OLTs?
OLTs are GPON network nodes that are located on the service providers’ side between Internet service providers (ISPs) and subscribers. They serve as traffic multiplexers, traffic signal converters and central control units in GPON networks. 

To function as expected in GPON networks, OLTs rely on the following modules:

* __An Ethernet interface__ works as the interface with the metro network. It is connected to the metro network. In downstream direction, the Ethernet interface classifies traffic from the metro network and transmits it to the GPON interface over switch fabric; in upstream direction, it aggregates traffic from the GPON interface and transmits it to the metro network.
  
* __A switch fabric__ works as the soft switch and central control unit for components in the GPON network.
  
* __A GPON interface__ works as the interface with the optical fiber. It is connected to ONTs at subscriber premises by the optical fiber. In downstream direction, it encapsulates the traffic with GPON encapsulation method (GEM) to enable it to travel to the subscribers over the optical fiber; in the upstream direction, it removes the encapsulation of the traffic and sends it the Ethernet interface over the switch fabric.

## What are ONTs?
ONTs are GPON network nodes that are located on the subscriber premises’ side between internet service providers (ISPs) and subscribers. They serve as optical fiber connection terminators, traffic signal converters and the interfaces with the subscribers. 

To provide different services, ONTs rely on the following interfaces:
* __An Ethernet interface__ provides data service
  
* __A video interface__ provides IPTV service

* __A voice interface__ provides voice service

__Note:__ An ONT is an instance of an Optical Network Unit (ONU), a generic term to denote the device that terminates an optical fiber connection and provides service to subscribers. An ONU usually refers to a multiple-subscribers device while the ONT is a single-subscriber device.