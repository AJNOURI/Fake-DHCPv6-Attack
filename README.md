fake-DHCPv6 attack
==================

The purpose of this scapy script is to check whether your DHCPv6 server is vulnerable to CPU and memory resources exhaustion.
A DHCPv6 server in Rapid-Commit mode attributes IPv6 prefix just by receiving unsollicited "SOLICIT" messages.

How to use the script:

1- Get the DHCPv6 sever MAC address by:
  - consulting the local neighbor table
  - pinging all DHCP agent multicast address FF02::1:2
2- Manually fill the script variable "macdst"
