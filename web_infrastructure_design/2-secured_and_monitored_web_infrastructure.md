# Secured and monitored web infrastructure
![Secured and monitored](https://i.imgur.com/cFNqvh9.png)
## Firewalls
 Firewalls protect the network by controlling what data can come in and go out, blocking unwanted or dangerous traffic to keep systems safe
## HTTPS
 HTTPS keeps the connection between  browser and  website secure by encrypting the data so nobody can spy on or steal important informations like passwords or credit card details
## Monitoring
- Monitoring is used to keep an eye on systems and applications to make sure they’re running smoothly, catch problems early, and fix them before they cause bigger issues
- To monitor the web server’s QPS, track how many requests it gets each second using tools or logs, then watch the numbers to spot any problems

---

# Issues
- Terminating SSL at the load balancer can be risky because the data between the load balancer and servers is not locked, so it might be seen or stolen if the network isn’t safe enough
- If there's only one MYSQL server to save data everything stops if it breaks down it also gets overwhelmed because it has to do all the work by itself
- If all servers handle everything, they get oveloaded fast and slow down and it's hard to fix or improve because everything is sharing the same block
