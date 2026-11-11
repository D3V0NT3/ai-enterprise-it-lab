# 02 — Virtual Network Configuration

## Objective

Create a shared virtual network for the Northstar Manufacturing lab,
supporting communication between lab machines and outbound internet access.

## Configuration

| Setting | Value |
| --- | --- |
| Platform | Oracle VirtualBox |
| Network type | NAT Network |
| Network name | Northstar-Corp-v2 |
| IPv4 subnet | 10.77.10.0/24 |
| Subnet mask | 255.255.255.0 |
| VirtualBox DHCP | Disabled |
| IPv6 | Disabled |

## Design Decisions

I selected NAT Network so the server and client can communicate
on the same virtual network and establish outbound connections.

VirtualBox DHCP is disabled because I will practise configuring
Windows Server DHCP in a later stage. Initially, I will assign
IP settings manually.

The existing host-only network was retained for the earlier lab.

## Configuration Evidence

![VirtualBox NAT Network settings](images/02-nat-network.png)

## Verification Status

The network name, subnet and disabled DHCP/IPv6 settings were
checked in VirtualBox Network Manager.

VM connectivity, DNS resolution and internet access have not yet
been tested. These checks will follow after the machines are deployed.

## Troubleshooting Note

Network Manager was initially hidden in Basic mode.
Switching VirtualBox to Expert mode exposed the network tools.

## Skills Practised

Virtual networking, IPv4 subnet configuration, DHCP planning
and technical documentation.

## Next Step

Create a fresh Windows Server VM and attach it to Northstar-Corp-v2.