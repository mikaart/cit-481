# Blog 1

Hello, in this series of blogs I will be talking about AWS and AWS associated services.

Today I will speak about **Identity Access Management** 

### IAM 101

IAM allows you to manage users and their level of access to the AWS Console.

IAM offers the following features:
```
Centralised control of your AWS account
Shared Access to your AWS account
Granular Permissions (meaning I want people to access this service but not the other one)
Identity Federation (Logging in to AWS console using your AD credentials or any other SSO)
Temporary access for users/devices and services
Integrated within other AWS services
```
There are 4 key terms associated with IAM. These are:

```
Users - end users such as People, employees of an organization, etc.
Groups - a collection of users. Each user in the group inherits the permission provided.
Roles - you create role and assign to AWS Resources
Policies - made up of documents, called Policy documents. These are written in JSON and give permissions to a User/Group/Role.
```

Here is an example of what a full allow Role looks like:

![Image](https://github.com/mikaart/cit-481/blob/master/images/blog1.1.PNG)

It is important to know that IAM is a universal service, unlike some other services in AWS. It applies to all regions at this time. 
New users have **NO** permissions when first created, besides the root user which is the account first created in AWS. That one has God powers.
New users are however provisioned with Access Key ID and Secret Access Key, which is not the same as password. You can use these to access AWS via APIs and Command Line. Also
remeber to set a 2FA authentication to your root account, as this is the key to your kingdom.