---
aliases: [ADSL, Fibre, WiFi, Bluetooth ]
tags: [GR10/Q4 computers/connectivity computers/connectivity ]
created: Fri 18/11 2022
---
# Communication Media
All networks are made up of 3 main parts:
- Sender/Source
- Receiver/Destination
- Connection between source and destination

The connection between two points is called a communication channel, or a transmission medium, and the sender and receiver are any kind of [[#Nodes]]. 

Communication channels have *bandwidth*. Bandwidth is the the maximum amount of data that can be transferred, usually measured in bits per second. Higher bandwidths create higher transmission rates. 

Bounded communication channels are often used for *LAN’s*, while unbounded communication channels are used for larger networks. 

## Bounded Transmission Media
There are 3 main categories of bounded transmission media we look at:
- Unshielded twisted pair (UTP)
- Shielded twisted pair (STP)
- Fibre-optic cable

### Unshielded Twisted Pair
These cables consist of multiple copper wires wound together to create a cable that is protected by a plastic casing. The twisting helps eliminate *interference* from the parallel signals. 

| Advantages                            |
| ------------------------------------- |
| Inexpensive                           |
| Fast Transmission rates               |
| Widely used – tested                  |
| Can be used in many types of networks |

| Disadvantages                                                |
| ------------------------------------------------------------ |
| Susceptible to interference                                  |
| Suffers attenuation – loss of signal quality due to distance |
| Crosstalk – corruption due to proximity to other data cables |

### Shielded Twisted Pair
A shielded twisted pair is the same as an unshielded twisted pair, but the strands within the cable are surrounded by plastic, reducing crosstalk and communication. 

| Advantages                                                      |
| --------------------------------------------------------------- |
| Fast Transmission rates                                         |
| No Crosstalk – corruption due to proximity to other data cables |
| Not Susceptible to interference                                 |

| Disadvantages                                                |
| ------------------------------------------------------------ |
| Expensive                                                    |
| Suffers attenuation – loss of signal quality due to distance |
| Can be used in many types of networks                        |

### Fibre Optic Cables
Fibre optic cables rely on light [[Transverse Pulses|pulses]] to transfer data. A central glass core surrounded by cladding that reflects the light back into the core is surrounded by padding to protect it. Light travels through the central core incredibly fast, and because there is a single line of data there is no interference or crosstalk. 

| Advantages                                                                      |
| ------------------------------------------------------------------------------- |
| Fast transmission rates because of the usage of light as a data transfer medium |
| More secure than UTP or STP because it is harder to ‘tap into’ light signals    |
| Can transmit over long distances without suffering attenuation                  |
| Unaffected by Interference of Crosstalk                                         |
| Immune to lightning or electrical surges                                        |

| Disadvantages                                          |
| ------------------------------------------------------ |
| Very Expensive to purchase or install                  |
| Strict certification standards make it hard to install |

#### Fibre optic cables as a backbone for interconnected LAN’s 
Fibre optic cables are often used to connect multiple LAN’s on different premises. 

## Unbounded Transmission Media
Unbounded transmission media send data without a physical connection through [[Mechanical Waves]] in the [[electromagnetic spectrum]]. These form wireless networks, where [[#Nodes]] are connected through waves, such as microwaves or radio-waves. Bluetooth is an example of one such wave. Each different signal uses a different [[Frequency (f)]] to differentiate them. 

We look at:
- Microwave transmissions
- Radio-wave transmitters

### Microwave Transmissions
Microwave transmissions use the line-of-sight method fro transmitting data between antennae, and can transmit very far providing there is no obstacle in the way. To avoid obstacles, we use satellites. 

> [!note]+ :spiral_notepad: terrestrial microwave transmissions
> microwave transmissions can be either terrestrial or satellite. terrestrial means land based, with transmission media being found on the ground and completely relies on a lack of obstacles between two points. 


Satellites are found in space, where they orbit the earth and transmit data. There are two types of orbit that are used for data transfers:
- Low earth orbit – faster speeds due to a closer orbit, but they move out of range every few hours.
- Geo-stationary orbit – a fixed position high above the earth, slower speeds but consistent


> [!tip]- :star_struck: Extra: Uses of different orbits
> geo-stationary orbits are well suited to television broadcasts, as latency is not an issue.
> 
> Low-earth orbits are well suited to interactive media, as they have low latency and a consistent connection. 

Satellites use *transponders* to send data to receiver stations located on the ground. these transponders receive signals, convert their frequencies, and then relay them to another station.  

### Radio Wave Transmissions
Radio waves are a terrestrial-based way to transfer information over short distances. However, they can pass through walls, making them very useful for [[Network Classifications#Home Networks]]. Wifi and bluetooth are uses of radio waves to transfer data. 