# Linux Networking

## Linux Commands

### grep Command

    1.1 How do you use the grep command to search for the word "error" in a file named "logfile.txt"?
    - `grep "error" logfile.txt`

    1.2 How can you search for a case-insensitive pattern using grep?
    - Add a `-i` ala `grep -i "error" logfile.txt`

### ping Command

    2.1 What is the purpose of the ping command and how do you use it to check connectivity to "google.com"?
    - The ping command will send ICMP Echo Request packets to the server and display the response times. 
    - `ping google.com`
    
    2.2 How can you limit the number of ping requests to 4?
    - Add `-c #` where # is 4 or the number of ping requests ala `ping -c 4 google.com`

### ssh Command

    3.1 How do you connect to a remote server with the IP address "192.168.1.10" using the ssh command with the username "user"?
    - `ssh user@192.168.1.10`
    
    3.2 How do you specify a different port (e.g., port 2222) for the ssh connection?
    - Add `-p <port>` ala `ssh user@192.168.1.10 -p 2222`

### RSA

    4.1 What is RSA and what is it commonly used for?
    - Its an algorithm for public-key cryptography, used for key based authentications on UNIX

    4.2 How do you generate an RSA key pair using ssh-keygen?
    - `ssh-keygen -t rsa`

### find Command

    5.1 How do you use the find command to locate a file named "example.txt" starting from the root directory?
    - `find /path -name "example.txt"`

    5.2 How can you find all files modified in the last 7 days using find?
    - Add `-mtime n` where n represents the number of days ago ala `find /path -mtime 2`

### Additional Commands

    6.1 What command is used to display disk usage statistics?
    - `df -T`

    6.2 How do you list all currently running processes?
    - `ps -e` or `ps -A` is generic UNIX
    - `ps -T` prints active processes that are executed from the terminal
    - `ps -C process_name` will filter list by the process name.

    6.3 How do you compress a file named "data.txt" using gzip?
    - `gzip data.txt`

## Networking Concepts

### TCP vs. UDP

    7.1 What is the main difference between TCP and UDP protocols?
    - TCP (transmission control protocol) is connection based & the UDP (user datagram protocol) is connectionless. TCP is more reliable but transfers data more slowly. UDP is less reliable but transfers data more quickly.

    7.2 Provide an example of an application that uses TCP and one that uses UDP.
    - TCP: Major internet applications like the World Wide Web, email, remote adminisration, and file transfers
    - UDP: Domain Name System (DNS), Streaming, Gaming, Swift Data Transfer, Virtual Private Networks (VPN)

### IP Addressing

    8.1 What is an IP address and what are the differences between IPv4 and IPv6?
    - Internet Protocol address is a unique string of characters that indentifies each computer using the IP to communicate over the network
    - IPv4 uses a 32-bit addresses, resulting in a limited pool.
    - IPv6 employs a 128-bit address, providing amount of unique IP addresses that should accommodate the ever-increasing device count

    8.2 How do you check your IP address on a Linux system?
    - `ifconfig` will list all IP addresses for each network interface in the computers networking layer
    - `ip addr` contains entries for wireless or WiFi adapters, wired or Ethernet adapters, and virtual adapters. Only one entry will usually contain the IP address

### Subnetting

    9.1 What is subnetting and why is it used?
    - Its a network inside a network. Subnets can make networks more efficient by shortening networking traffic without having to pass through unnecessary routers.

    9.2 How do you calculate the subnet mask for a network with a prefix of /24?
    - Convert /24 to binary: 11111111.11111111.11111111.00000000
    - Fill in the subnet mask: 255.255.255.0 

### DNS

    10.1 What is DNS and how does it work?
    - Domain Name System, which is a system that translate domain names into IP addresses that browsers use to load web pages

    10.2 How do you query DNS records for a domain using the dig command?
    - `dig [server] [name] [type]`

    10.3 What is a Fully Qualified Domain Name (FQDN)?
    - a domain name that specifies the exact location of a computer or internet host in the Domain Name System's tree hierarchy

    10.4 What is a CNAME record in DNS and what is it used for?
    - Maps an alias name to a true or canonical domain name

### Routing

    11.1 What is the purpose of a routing table in a network?
    - to help routers make effective routing decisions, whenever a packet is sent through a router to be forwarded to a host on another network, the router consults the routing table to find the IP address of the destination device and the best path to reach it

    11.2 How do you view the routing table on a Linux system?
    - `route -n`

### Network Troubleshooting

    12.1 What command would you use to trace the path packets take to a network destination?
    - `traceroute` command

    12.2 How do you display all network interfaces and their configurations?
    - `hwinfo` command
