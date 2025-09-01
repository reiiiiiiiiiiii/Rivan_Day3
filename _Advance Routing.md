
<!-- Your monitor number = #$34T# -->


## ⛅ Warm Up for Day 3.

<br>

### 🔧 Configure the following:
  - Switch (__CoreTAAS__ & __CoreBABA__)
  - Voice Gateway/Call Manager (__CUCM - Cisco Unified Call Manager__)
  - Router (__EDGE__)

<br>

## 🎯 Review

### 1. What is the reason for the error?

~~~
Router(config)# interface GigabitEthernet 1/0/1
Router(config-if)# ip add 192.168.16.143 255.255.255.240
Bad Mask /28 for address 192.168.16.143
~~~

&nbsp;
---
&nbsp;

### 2. Devices fail to obtain IP addresses from a DHCP server. Determine the issue by going through the dhcp configurations shown below.

~~~
Router# show run | s dhcp
ip dhcp excluded-address 10.28.0.1 10.28.0.100
ip dhcp pool mainpool
 network 10.28.0.0 255.255.255.248
 default-router 10.28.0.1 
 domain-name main.com
 dns-server 10.28.1.10
~~~

&nbsp;
---
&nbsp;

### 3. Match the Host addresses on the left to their correct IP range on the right.

|     | Host                |         ---        |     | Range (1st Valid - Broadcast)     |
| --- | ---                 | ---                | --- | ---                               |
| 1   | 10.187.45.21 /14    |                    | A   | 192.168.100.193 - 192.168.100.223 |
| 2   | 10.180.201.90 /12   |                    | B   | 10.176.0.1 - 10.191.255.255       |
| 3   | 172.16.74.5 /20     |                    | C   | 172.16.64.1 - 172.16.79.255       |
| 4   | 172.16.81.1 /19     |                    | D   | 192.168.100.193 - 192.168.100.208 |
| 5   | 192.168.100.203 /27 |                    | E   | 10.184.0.1 - 10.187.255.255       |
| 6   | 192.168.100.195 /28 |                    | F   | 172.16.64.1 - 172.16.95.255       |

&nbsp;
---
&nbsp;

### 4. Design a network for Cognizant.com with 4720 potential users. Use the IP address space 10.42.0.0 /16

C:
S:
I:

| Cognizant.com     | IPv4  |
| ---               | ---   |
| Network           |       |
| First Valid       |       |
| Last Valid        |       |
| Last IP/Broadcast |       |
| ---               | ---   |
| NOT Cognizant.com |       |

