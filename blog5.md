# Blog 5

Hello, today in my blog I will be talking about VPC.

## What is VPC

Amazon Virtual Private cloud lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define. You have complete control over your virtual netoworking environment, including selection of your own IP address range, creation of subnets, and configuration of route tables and network gateways. You can create a public-facing subnet for your webserver that has access to the Internet, and place your backend systems such as databases or application servers in a private-facing subnet with no Internet access. You can leverage multiple layers of security, including security grou[s and network access control lists, to help control access to Amazon EC2 instances in each subnet.

![Image](https://github.com/mikaart/cit-481/blob/master/images/5.2.PNG)


### VPC Functionality

With VPC, we are able to complete a few networking tasks in attmept to setup our secure environment:

```

1.   Launch Instances into a subnet of your choosing
2.   Assign custom IP addresses ranges in each subnet
3.   Configure route tables between subnets
4.   Create internet gateway and attach it to our VPC
5.   Instance security groups
6.   Subnet network ACL's

```

You could use Default VPC as it is user friendly and allows you to immediately deploy instances, automatically assigning EC2 instance with a both public and private IP address.

So VPC is basically a logical datacenter, consisting of Private Gateways, Route Tables, Network ACL's, Subnets, and Security groups.
Security groups are stateful, Network ACL's are Stateless.