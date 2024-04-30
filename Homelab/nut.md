## NUT Server 1   -  Outlet group 1
	- Begins Shutdown Sequence after 5 minutes
	- Talos nodes shutdown immediately
	- Proxmox Nodes shutdown after 5 minutes to give talos time to go down gracefully
	- NTP Server 1 exists on one of the proxmox nodes.
	- No permision to shutdown the UPS
	- Outlet group 2 set to turn off 

## NUT Server 2 - Outlet group 2
	- Doesn't do anything until low battery signal then issues FSD
	- Controls OPNsense
	- Keeps network and internet alive as long as possible

## Useful Commands
`upsc apc@localhost` - Show the status of the APC ups.