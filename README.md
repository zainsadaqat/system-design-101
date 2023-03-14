# System Design 101

## Browser/Client
For Example: Client searches https://facebook.com --- Browser send a request to Facebook's Server ---> Facebook Server.
Facebook Server processes the request and sends the response back to the client in form of HTML, CSS, JS.

But facebook receives billions of requests every single day and it's not possible for a single web server to handle this.

## DNS (Domain Name System)
DNS stores IP address of websites. For Example: when a user searches for Facebook. it goes to DNS and translates the http://facebook.com to its IP address. it can be of IPv4 or IPv6 and DNS is handling it. A website can own many IP addresses. 

## Web Server
- application logic
- database

Vertical Scaling:- Increasing resources on 1 server For Example: increasing the amount of Memory, Storage, Network Speed and Processing Power (CPU) for a single web server.

Horizontal Scaling:-
