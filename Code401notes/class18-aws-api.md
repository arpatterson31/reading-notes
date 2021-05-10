# Class 18 Reading: AWS: API, Dynamo, and Lambda

## Review, Research, and Discussion

### What are serverless functions?

- single-purpose, programmatic functions that are hosted on managed infrastructure. These functions, which are invoked through the Internet, are hosted and maintained by cloud computing companies. The engineering teams within those companies ensure that the serverless functions have near-perfect uptime, redundant instances around the world, and scale to any incoming network request volume.*[source](https://www.pubnub.com/blog/what-is-a-serverless-function/)*

### If you were to create a system that emulated Lambda functions, how would you do it?

- You could use serverless functions or you could create a CL tool to locally run and remotely deploy your node.js applications *[source](https://stackoverflow.com/questions/34196043/are-there-any-emulator-for-aws-lambda/34499308)*

### Describe how a CDN works

- CDNs work through servers nearest to the website visitor respond to the request. The content delivery network copies the pages of a website to a network of servers that are spread out at geographically different locations, caching the contents of the page. When a user requests a webpage that is part of a content delivery network, the CDN will redirect the request from the originating site’s server to a server in the CDN that is closest to the user and deliver the cached content. CDNs will also communicate with the originating server to deliver any content that has not been previously cached. In turn, the speed is improved by distributing content closer to the website visitors by using a nearby CDN server, causing visitors to experience faster page loading times. In simpler terms, for example, instead of a user in London trying to access a server in LA, which can cause slower Internet speeds, the user would be redirected through a CDN that is geographically closest to them (London, Paris, Stockholm, etc). As of today, the majority of web traffic goes through through CDNs, including traffic from major sites like Facebook, Netflix, and Amazon. *[source](https://cyberhoot.com/cybrary/content-delivery-network-cdn/)*

## Document the following vocab words

- **Serverless functions:** single-purpose, programmatic functions that are hosted on managed infrastructure. These functions, which are invoked through the Internet, are hosted and maintained by cloud computing companies. The engineering teams within those companies ensure that the serverless functions have near-perfect uptime, redundant instances around the world, and scale to any incoming network request volume.*[source](https://www.pubnub.com/blog/what-is-a-serverless-function/)*
- **Cloud Storage:** a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service. It’s delivered on demand with just-in-time capacity and costs, and eliminates buying and managing your own data storage infrastructure. This gives you agility, global scale and durability, with “anytime, anywhere” data access. *[source](https://aws.amazon.com/what-is-cloud-storage/)*
- **CDN:** Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos. *[source](https://cyberhoot.com/cybrary/content-delivery-network-cdn/)*

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- I haven't heard of Amazon API or DynamoDB but I'm excited to learn more about them. I have used MongoDB as a NoSQL db so hopefully there isn't a huge difference.

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- DynamoDB, hopefully it will be easy to use like MongoDB. But I'm excited to be learning other NoSQL dbs

### What are you most excited about trying to implement or see how it works?

- Dynamoose, not only does it have great name, but if its easy like mongoose was for MongoDB, I'm all for it!
