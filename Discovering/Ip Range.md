### Ip range scanning
If you didnt read the e file, you might take a look it.
Scanning just an ip, probably will not get any port. This is because the network have a  dedicated ip for the servers.
Most users buys a dedicated ip for each server for more protection.
Lets put an eg:
192.1.2.3 -> 25565 service: Minecraft version: "Welcome to rinkcraft network"
192.1.2.4 -> 25569 service: Minecraft version: "Survival rinkcraft network"
As you can see, the survival modality of the server, have other ip and port.
So, scanning an ip range, we will try to find the hidden modality.
Eg of a ip range scan:
nmap 192.1.2.* --open -p 25565
In this case I am using nmap, but you can use other tools.
What I am saying in the scan, is that to scan all the range of ips, and give me it the ips that have the 25565 port open.
And then, you can manually check the ports to find the server of the modality.
Now, doing this, you might find other servers/network that dont belong the network target, with 0 players, with other version, that you probabyly you are not interested.
Here come Qubo scan to help, Qubo scan acts like a scanner and checker at the same time. That why I dont recommend you to use nmap.
As I sayed, with qubo you can add arguments like min of players, version of the server, to clean the junk server.
This with nmap, masscan, angry ip or other tools you cant.
Other people, use the nmap to get ips with a specific port(s), and then, with her own checker, get the servers.
This I will talk it on the future.
### Second ip range




