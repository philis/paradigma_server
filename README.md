# paradigma_server
This is a server that receives data from a systa comfort 2 heating and stores it into a mysql database.

The server requires a DHCP server (can be hosted on the same machine as the server itself) that issus a IP address to the SystaComfort2. Additionally the DHCP server must pass information about the DNS server to use. This DNS-Server must map paradigma.remoteportal.de to the machine the server runs on.

The server listens to Data arriving from the SystaComfort2 on port 22460. It responds to the packages which then forces the SystaComfort 2 to send additional packages that contain information about the  current heating parameters.
