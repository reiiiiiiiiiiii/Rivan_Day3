
# Access RSTHayup Labs

### Prerequisites
- Terminal Emulator (Putty or __SecureCRT__)
- Type 2 Hypervisor (VMWare __Workstation__)
- __RSTHayup VM__
- Downloaded Repository __Rivan_Day3__

<br>
<br>

---
&nbsp;

## Setup the Virtual Workspace

### 1. On VMWare Workstation, go to `Edit` > `Virtual Network Editor..`

<br>

![00_AccessRST](img/00.JPG)

&nbsp;
---
&nbsp;

### 2. Select `Add Network..`

<br>

![01_AccessRST](img/01.JPG)

&nbsp;
---
&nbsp;

### 3. Add `VMnet15`

![02_AccessRST](img/02.JPG)

&nbsp;
---
&nbsp;

### 4. Edit VMnet15 with the following settings:
- VMnet Information: __Host-only__
> - [x] Connect a host virtual adapter to this network
> - [x] Use local __DHCP service__ to distribute IP address to VMs
- Subnet IP: 10.255.10.0
- Subnet Mask: 255.255.255.0

![03_AccessRST](img/03.JPG)

&nbsp;
---
&nbsp;

### 5. Now `Add Network..` again

![04_AccessRST](img/04.JPG)

&nbsp;
---
&nbsp;

### 6. Add `VMnet16`

![05_AccessRST](img/05.JPG)

&nbsp;
---
&nbsp;

### 7. Edit VMnet16 with the following settings:
- VMnet Information: __Host-only__
> - [x] Connect a host virtual adapter to this network
> - [x] Use local __DHCP service__ to distribute IP address to VMs
- Subnet IP: 10.69.255.0
- Subnet Mask: 255.255.255.248

![06_AccessRST](img/06.JPG)

&nbsp;
---
&nbsp;

### 8. Extract the `RSTHayup` 7zip file
> [!NOTE]
> The filename may be different.

<br>

![07_AccessRST](img/07.JPG)

&nbsp;
---
&nbsp;

### 9. Inside the RSTHayup directory, open the `.vmx` file.

![08_AccessRST](img/08.JPG)

&nbsp;
---
&nbsp;

### 10. Power on the Virtual Machine
> [!NOTE]
> If you do not create VMNets 15 & 16, RSTHayup VM will take a while in obtaining IP address for its ethernet interfaces.

![09_AccessRST](img/09.JPG)

&nbsp;
---
&nbsp;

### 11. Select `I copied it`

<br>

![10_AccessRST](img/10.JPG)

&nbsp;
---
&nbsp;

### 12. Login to the VM
- Username: root  
- Password: C1sc0123  

&nbsp;
---
&nbsp;

### 13. Delete the Firewall
Enter the following command:
~~~
rm -rf /etc/udev/rules.d/70-persistent-net.rules
~~~

Then, 

~~~
reboot
~~~

<br>

> [!TIP]
> Press `[TAB]` to autocomplete.
> `Example: rm -rf /e[TAB]/u[TAB]/r[TAB]/7[TAB]`

<br>

![11_AccessRST](img/11.JPG)

&nbsp;
---
&nbsp;

### 14. Access the GUI
After the VM has rebooted, it will recieve an IP address.  
In this case, it is 208.8.8.129

<br>

![12_AccessRST](img/12.JPG)

<br>

Open the IP address on a browser.

&nbsp;
---
&nbsp;

### 15. Select `00 RSTvX: RouteSwitchTshoot Hayup Lab`

<br>

![13_AccessRST](img/13.JPG)

&nbsp;
---
&nbsp;

### 16. The first page will be the topology. To turn on the devices, select the `Devices` tab.

<br>

![14_AccessRST](img/14.JPG)


&nbsp;
---
&nbsp;

### 17. Power on all the devices at once.

<br>

![15_AccessRST](img/15.JPG)

<br>

![16_AccessRST](img/16.JPG)

&nbsp;
---
&nbsp;

### 18. 

