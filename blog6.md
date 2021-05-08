# Blog 6

Hello, today I will be talking about Load Balancer in AWS.

## Load Balancer 101

It's a virtual device designed to balance the load from the webservers or applications.

**Load balancing types in AWS:**

```

1.  Application Load Balancer
2.  Network Load Balancer
3.  Classic Load Balancer

```

![Image](https://github.com/mikaart/cit-481/blob/master/images/blog6.1.PNG)


Application Load Balancers are best suited for Load balancing of HTTP/S traffic. They operate at Layer 7 (Application) and are application-aware. They are intelligent, and you can create advanced request routing, sending specified requests to specific web servers. You can utilize such tools as X-Forwarded-For header and others for applications with user specific IP.

Network Load Balancers are best used for load balancing of TCp traffic where extreme performance is required. Operating at the Layer 4 (Network), Network Load Balancer are capable of handling millions of requests per second, while maintaining ultra-low latencies. For extreme performance only.

Classic Load Balancers are the legacy Elastic Balancers. You can load balance HTTP/s applications and use Layer 7 specific features, such as sticky sessions. You can also use strict Layer 4 load balancing for applications that rely purely on the TCP protocol.