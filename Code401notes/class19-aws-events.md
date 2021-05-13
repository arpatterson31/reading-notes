# Class 19 Reading: AWS: Events

## Review, Research, and Discussion

### Describe the similarities between AWS API Gateway + Lambda and ExpressJS Server

- AWS API allows you to create CRUD actions and routes. Lambda are the functions that trigger from the CRUD action. The ExpressJS server is all those in one application.

### List the AWS Database Offerings and talk about the pros and cons of each

- [AWS Databases](https://aws.amazon.com/products/databases/)

- Pros
  - integrate with other AWS services
  - no hardware maintenance needed
  - automated backups

- Cons
  - price
  - no scale out
  - performance is not guaranteed

### Whats the difference between a FIFO and standard queue?

- FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing. FIFO queues provide additional features that help prevent unintentional duplicates from being sent by message producers or from being received by message consumers *[source](https://aws.amazon.com/about-aws/whats-new/2016/11/amazon-sqs-introduces-fifo-queues-with-exactly-once-processing-and-lower-prices-for-standard-queues/#:~:text=FIFO%20queues%20have%20essentially%20the,being%20received%20by%20message%20consumers.)*

### How can the server be assured a message was properly received?

- TCP/IP cannot guarantee that all data that have been sent will also be received. But even if it would guarantee it that is not what you need. What sender actually needs is to know if it does not have to send data again, and that usually implies if sent data has been processed on receivers side.
If sender needs to know this then communication protocol must be changed so that sender can receive a confirmation by the receiver that it can safely assume that data has been processed. Also, sender must at certain point proclaim a time-out (and close the socket) if receiver did not send back the confirmation on time (and in your code you must decide what to do about it, maybe save data to be sent at later time, or raise an alert to the user). Also receiver must handle the situation where the same data is being sent twice (as last item in previous connection, and as another item in new connection) and not treat this data as two distinct pieces of data. *[source](https://stackoverflow.com/questions/16731849/check-if-data-has-been-received-socket-c-sharp)*

## Document the following vocab words

- **Serverless API:** Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. A serverless application runs in stateless compute containers that are event-triggered, ephemeral (may last for one invocation), and fully managed by the cloud provider. *[source](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)*
- **Triggers:** Triggers are pieces of code that will automatically respond to an event. *[source](https://dashbird.io/blog/what-are-aws-lambda-triggers/#:~:text=Triggers%20are%20pieces%20of%20code,ARN%20with%20your%20Lambda%20function.)*
- **Dynamo vs Mongo:** Both are NoSQL Dbs, Dynamo is AWS DB in the cloud
- **Dynamoose vs Mongoose:** Dynamoose is the model handler for DynamoDB and Mongoose is that for MongoDB

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- I haven't heard of Amazon SQS or SNS so these are newer concepts for me to learn

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- All since I don't have any experience with it

### What are you most excited about trying to implement or see how it works?

- SQS and SNS
