# WORK IN PROGRESS (DonkeyTracker Workshop)
Workshop to build an end-to-end serverless tracking application for your mobile device including a serverless backend powered by Amazon Web Services (AWS). The keyword here is **serverless**.

**Serveless computing** allows you to focus entirely on your application rather than managing servers and scaling the environment. Often it is also more cost efficient since you avoid overprisioning and have just the right capacity. Therefore this workshop is build around technologies such as DynamoDB, Lambda, API Gateway and Simple Storage Service (S3).

## Requirements

* An **AWS Account**. If you don't have one yet, head over to [Appendix 3](./Appendix-03) to learn how to get one and configure the initial Identity and Access Management. You will also need an **AWS Access Key ID** and **AWS Secret Access Key** for some of the testing from the AWS CLI. [Appendix 3](./Appendix-03) also explains how to get the key.
* A **Code Editor**. I prefer [Visual Studio Code](https://code.visualstudio.com/) and use the following extensions for this workshop:
    * [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) for the documentation in Markdown

## Step 1: Persisting Data in DynamoDB Table

AWS provides many options to store and query data. For the type of data that we want to store in our tracking application, a database is probably most appropriate and AWS provides severeal managed and unmanaged services. While the recently announced [Amazon Aurora Serverless](https://aws.amazon.com/blogs/aws/in-the-works-amazon-aurora-serverless/) might be an option in the future we'll pick for now the already proven NoSQL database [DynamoDB](https://aws.amazon.com/dynamodb/). 

Head over to [Step 1](./Step-01) to dive right in.

## Step 2: Writing Data to DynamoDB Table with Lambda

AWS [Lambda](https://aws.amazon.com/lambda/) lets you run code without provisioning or managing servers. You pay only for the compute time you consume - there is no charge when your code is not running. 

Lambda truely simplifies the development as long as your code meets the requirements, i.e. if you're developing APIs that don't require more than 5 min of execution time or 3 GB of memory it is pefect to get started quickly, avoid the management of servers and save cost.

It is outside the scope of this workshop but for more complex scenarios where you may want to orchestrate multiple Lambda functions, have a look at [AWS Step Functions](https://aws.amazon.com/step-functions).

For now head over to [Step 2](./Step-02) to create your Lambda function.

## Step 3: Exposing your Lambda Function through the API Gateway

[coming soon]

## [Appendix 1: References](./Appendix-01)
## [Appendix 2: Acronyms](./Appendix-02)
## [Appendix 3: Initial Identity and Access Management for a New Account](./Appendix-03)
