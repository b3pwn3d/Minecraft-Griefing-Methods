### Ip range scanning
If you didnt read the e file, you might take a look it.
Scanning just an ip, probably will not get any port. This is because the network have a  dedicated ip for the servers.
Most users buys a dedicated ip for each server for more protection.
Lets put an eg:

192.1.2.3 -> 25565 service: Minecraft version: "Welcome to rinkcraft network" 

192.1.2.4 -> 25569 service: Minecraft version: "Survival rinkcraft network"

As you can see, the survival server of the network, have other ip and port.
So, scanning an ip range, we will try to find the hidden modality.
Eg of a ip range scan:

nmap 192.1.2.* --open -p 25565

In this case I am using nmap, but you can use other tools.
What I am saying in the scan, is that to scan all the range of ips, and give me it the ips that have the 25565 port open.
And then, you can manually check the ports to find the server of the modality.
Now, doing this, you might find other servers/network that dont belong the network target, with 0 players, with other version, that you probabyly you are not interested.
Here come Qubo scan to help, Qubo scan acts like a scanner and checker at the same time. Thats why I dont recommend you to use nmap.
As I sayed, with qubo you can add arguments like min of players, version of the server, to clean the junk server.
This with nmap, masscan, angry ip or other tools you cant.
Other people, use the nmap to get ips with a specific port(s), and then, with her own checker, get the servers.
This I will talk it on the future.
### Advanced ip range scan
As I told you before, you can perfom a ip range, but you can expand the ip range for better results.
Instead of using 192.1.2.* you can try with 192.1. *. *  
Expanding the range, you will get much more servers, instead using just a range.

The bad of this types of scanning, is that will take a lot of time to perfom it. We are talking about 1 hour to scan that type of range.
And having your pc on so much, idk that is a good idea.
So, I will explain you, how to do it more easy and practical

### Using a vps to scanning
Getting a vps is really easy. You can get a really cheap one for 2 3 $.
If you dont wanna pay for one, you can try hacking some SSH server to acces them and build your scanners there.
Your vps should be a linux system, to be more faster.
Once you have the vps, you can now start to perfom the scan with the qubo scanner.
Remember to save the procces in second plan, so when you close the ssh connection, the task doesn`t kill



