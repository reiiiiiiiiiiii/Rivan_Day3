
# Access RSTHayup Labs

## Setup the Virtual Workspace


1. Create and Configure VMNets 15 & 16
- VMWare > Virtual Network Adapter
- Add Network
- Select VMNet15
- Modify VMNet15 with the following:
- Add another Network
- Select VMNet16
- Modify VMNet16 with the following:
- Apply and Finish.


2. Download and extract the _RSTHayupV4.7z file.

3. Inside the _RSTHayupV4 directory, open the .vmx file.

4. Power on the Virtual Machine
> ![Note] If you do not create VMNets 15 & 16, _RSTHayupV4 VM will take a while in obtaining IP address for its ethernet interfaces.

5. Select 'I copied it!'

6. Login:
- Username: root
- Password: C1sc0123

7. Delete the Firewall

Enter the following command:
rm -rf /etc/udev/rules.d/70-persistent-net.rules

Then, reboot.

> ![Tip] Press [TAB] to autocomplete. Example: rm -rf /e[TAB]/u[TAB]/r[TAB]/7[TAB]


8. Access the GUI
After the VM has rebooted, it will recieve an IP address.


Open the IP address on a browser
- Select 00 RSTvX: RouteSwitchTshoot Hayup Lab

