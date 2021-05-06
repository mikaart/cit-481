# Blog 2

Hello, today we will be talking about S3 and basics of what it represents

## S3 101

S3 provides developers and IT teams with secure, durable, and highly-scalable object storage. Amazon S3 is easy to use, with a simple web services interface to store and retrieve any amount of data form anywhere on the web. This means that S3 is a place where you would store flat files (pdf, txt, html, etc.) with that data being stored on backend of AWS.

The files are stored within a bucket (or a folder), with a maximum capacity of each file being 5TB, however having general unlimited storage. It is also important to remember that S3 buckets are named universally, meaning that the names assigned are unique and cannot repeat. 

### Keys, terms, and understanding the service

Some of the important terms associated with the S3 container and its files are:

```
Key - the name of the object
Value - the data made up of sequence of bytes
Version ID - Important for versioning
Metadata - info parameters about data you store
```


Amazon guaranteed 99.99% availability for the S3 platform (which is high for SLA measurements), as well as 99.99999999999% of durabilty, meaning if the object is being uploaded in the S3, it is not going to be lost. 

As soon as you upload the object, you will be able to read it immideately. But if you update the object or delete an object you might get an older version of that file or object. This has to do with S3 Eventual Consistency, which basically means objects take some time to propogate and in that time older version of the object will be utilized.

With that said, there are different ways to go about storing data on S3. AWS allows for different Tiered Storages, depending on your needs and desired costs. One can use lifecycle management (switching from one tier to another by expiration time) in order to better distribute important files. It is important to use services smartly with AWS. There is encryption being allowed as well, so you can encrypt the files and also use ACL's to limit access to buckets for only those that are authorized.


Here is an image with Available Tiered Storages:

![Image](https://github.com/mikaart/cit-481/blob/master/images/blog2.1.PNG)

Looking above, S3 Interlligent Tiering is the best optimized tier as it optimizes costs by automatically moving data to the most cost-effective access tier, without performance impact or operational overhead.
