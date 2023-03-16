# System Design 101

## Browser/Client
For Example: Client searches https://facebook.com --- Browser send a request to Facebook's Server ---> Facebook Server.
Facebook Server processes the request and sends the response back to the client in form of HTML, CSS, JS.

But facebook receives billions of requests every single day and it's not possible for a single web server to handle this.

## DNS (Domain Name System)
DNS stores IP address of websites. For Example: when a user searches for Facebook. it goes to DNS and translates the http://facebook.com to its IP address. it can be of IPv4 or IPv6 and DNS is handling it. A website can own many IP addresses. 

## Web Server
Web servers run some application logic and has access to the database.
Application logic lives inside the web server but the database is external to the web server.
`application logic`, `database`

- Vertical Scaling:- Increasing resources on 1 server For Example: increasing the amount of Memory, Storage, Network Speed and Processing Power (CPU) for a single web server.

- Horizontal Scaling:- Duplicate or Clone web server multiple times virtually. Cloning web servers will have the same application logic that will connect with the same one database.

- Latency:- the time a request takes for the browser to fire a request and get back the response from the server. The total travel time is Latency.

## Load Balancer
Equally distributes the received requests between the web servers. The load can be distributed using the a strategy called Round Robin. If a server goes downn then it won't route any request to that server rather it will distribute the requests to the remaining web servers. Load balancer actually works like a Traffic Cop (Traffic Policer Officer)
- Session Persistance ( Session between a user and a web server)
