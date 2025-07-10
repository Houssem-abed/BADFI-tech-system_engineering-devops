# Distributed Web Infrastructure

![System Diagram](https://i.imgur.com/mycKYaL.png)

## How It Works
This setup shares website traffic between two servers using a load balancer to handle more visitors and prevent overloads

## Main Parts

### Traffic Distribution
- Uses HAProxy load balancer
- Sends requests to servers one after another (Round Robin)
- Normally uses just the main server (Active-Passive)
- Backup server takes over if main server fails

### Database Setup
- Main database handles all data changes
- Backup database helps with reading data
- Changes automatically copy from main to backup

## Issues

### Weak Points
- If load balancer fails website goes down
- If main database fails can't save changes

### Security Issues
- Data sent without encryption
- No protection against hackers

### Missing Monitoring
- Can't check server health
- No alerts for problems
