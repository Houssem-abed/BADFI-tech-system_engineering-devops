# Distributed Web Infrastructure

![System Diagram](https://i.imgur.com/mycKYaL.png)

## How It Works
- This setup shares website traffic between two servers using a load balancer to handle more visitors and prevent overloads

## Round Robin Algorithm
- The load balancer uses Round Robin, which means it sends each new request to the next server in a simple cycle


## Database Setup
- My load balancer is set by default Active-Active
## The difference between the two sets
- Active - Active : All Load balancers are working on the same time equally if one fails the other will keep handling the requests without interruption
- Active-Passive: Only one load balancer is active and handling traffic while the other is on standby, so if the active one fails automatically the passive takes over

---

## Issues
### Where are SPOF
- If load balancer fails website goes down
- If main database fails can't save changes
### Security Issues
- Data sent without encryption (no HTTPS)
- No protection against hackers (No Firewall)
### Missing Monitoring
- Can't check server health
- No alerts for problems
