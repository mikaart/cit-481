# Blog 4

Greetings, today we will be talking about CloudWatch and CloudTrail and things important to know around it. (including physical implementations)

## CloudWatch

Amazon CloudWatch is a monitoring service to monitor your AWS resources, as well as the applications that you run on AWS. It monitors performance of Compute group such as EC2 Instances, Autoscaling Groups, Load Balancers, as well as Storage and Content Delivery.

Some of the metrics being monitored include:

```
CPU
Network
Disk
Status Check
```

AWS CloudTrail increases visibility into your user and resource by recording AWS Management Console actions and API calls. You can identify which users and accounts called AWS, the source IP address from which the calls were made, and when the calls occured. By default it monitors events every 5 minutes, which can be switched by enabling detailed monitoring. 

![Image](https://github.com/mikaart/cit-481/blob/master/images/blog4.1.PNG)


It is important to remember that CloudWatch monitors performance compared to CloudTrail which monitors API calls in the AWS platform. So while CloudWatch is all about performance, CloudTrail is all about auditing. It means the network throughput or EC2 status check will be on CloudWatc


![Image](https://github.com/mikaart/cit-481/blob/master/images/blog4.2.PNG)
