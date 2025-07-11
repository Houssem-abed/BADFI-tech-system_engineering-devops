# Scale Up
![Scale up](https://i.imgur.com/R22fZ95.png)

## Some specifics about this infrastructure
### Ative and Passive Load Balancers
- We used two Load Balancers (Active-Passive) so the system stays online if one fails, The active handles traffic normally and the passive takes over if something goes wrong
### Firewalls
- We added Firewalls to protect each part of the system to make sure everything follows the right path
### SSL certificates
- We added SSL certificates to make sure that all our communication is encrypted even between servers
### Monitoring
- We installed monitoring tools on each server to keeo an eye on performance usage and issues if they exists and splitted them to make things more reliable
### Separate servers web, app and database
- We seperated servers for web server, application server and database server to keep things running smoothly so if the traffic grows, we can upgrade the web servers only
### Floating Ip
- The floating IP points to the active load balancer and if the active one fails it redirects to the passive without needing to change the IP