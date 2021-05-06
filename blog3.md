# Blog 3

Greetings, today I am going to be talking more about CloudFront and what it represents of itself


### Intro

**Edge location** is the location where content will be cached. This is separate to an AWS Region/AZ.

**Origin** is the origin of all the files that the CDN will distribute such as S3 bucket, EC2 instance, Elastic Load Balancer, or Route53.

**Distribution** is the name given the CDN which consists of a collection of Edge Locations.


### CloudFront     

CloudFront is a content delivery network which serves as a system of distributed servers (network) that delivers webpages and other web content to a user based on the geographic locations of the user, the origin of the webpage, and a content delivery server. 

Say there is a website hosted in London and we have a set of users all around the world. Withoud CDN (CloudFront) enabledf, every user has to always connect to that one server and always pull data directly from there, meaning extra traffic and redundancy. 

With CloudFront, you are able to use a network of Edge Locations which set up around the world and stored the cached information of whatever hosted service on there, including dynamic, static, streaming, and interactive content. Requests for the content are automatically routed to the nearest edge location, so content is delivered with the best possible performance. That said, you can setup either regular or Web Distributions, which are used for websites.

The edge locations are also Read/Write enabled, meaning that you can edit the corrupted cache as an Admin if needed.