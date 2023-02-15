- Parameters such as TTL and TCP window size in the IP header of the first packet in a TCP session plays an important role in identifying the OS running on the target machine. The TTL field determines the maximum time a packet can remain in a network, and the TCP window size determines the length of the packet reported. These values differ for different OSes: you can refer to the following table to learn the TTL values and TCP window size associated with various OSes.
	- ![[https://github.com/Indrajith-S/CEH-Notes/blob/993b7f77cc0a86f42ee0800ace0de9a0be954115/Images/Pasted%20image%2020220720235539.png]]

- Using Nmap- Zenmap GUI
	> nmap --script smb-os-discovery.nse #ip


	- **--script**: specifies the customized script and **smb-os-discovery.nse**: attempts to determine the OS, computer name, domain, workgroup, and current time over the SMB protocol (ports 445 or 139).
