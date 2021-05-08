# Blog 10

Hello, today I will be talking about AWS Lambda

## What is Lambda   

AWS Lambda is a compute service where you can upload your code and create a Lambda function. AWS Lambda takes care of provisioning and managing the servers that you use to run the code. you don't have to worry about operating systems, patching, scaling, etc.

You can use it as an event-driven compute service where AWS Lambda runs your code in respone to events. These vents could be changes to data in an Amazon S3 bucket or an Amazon DynamoDB table. Or you can use it as a compute service to run tour code in response to HTTP requests using Amazon API Gateway or API calls made using AWS SDKs. 


### Pricing

**Number of requests**

First 1 million requests are free. AWS then charges $0.20 per million requests.

**Duration**

Duration is calculatd from the time your code begins executing until it returns or otherwise terminates, rounded up to the nearest 100ms. The price depends on the amount of memory to your function. But charges are insignificant overall ($0.00001667)
