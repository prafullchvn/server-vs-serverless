# Disadvantage of Serverless

## Response latency

Response latency is the time between when a request is stimulated and when a program reacts. In the cloud, serverless computing is not continually running—it gets powered down between requests.

As a result, having to start from dormant serverless code can cause response latency. It can take as long as several seconds to spin up and process code.

## Security

When vendors run the entire backend, it may not be possible to fully vet their security, which can especially be a problem for applications that handle personal or sensitive data.

Because companies are not assigned their own discrete physical servers, serverless providers will often be running code from several of their customers on a single server at any given time. This issue of sharing machinery with other parties is known as 'multitenancy'.
Multitenancy can affect application performance and, if the multi-tenant servers are not configured properly, could result in data exposure.

## Testing

In a non-Serverless world, developers often have local analogs of application components (like databases, or message queues) which can be integrated for testing in much the same way the application might be deployed in production. Serverless applications can, of course, rely on unit tests, but more realistic integration or end-to-end testing is significantly more difficult.
The difficulties in local testing of Serverless applications can be classified in two ways. Firstly, because much of the infrastructure is abstracted away inside the platform, it can be difficult to connect the application components in a realistic way, incorporating production-like error handling, logging, performance, and scaling characteristics. Secondly, Serverless applications are inherently distributed, and consist of many separate pieces, so simply managing the myriad functions is challenging.

## Debugging

Every time a serverless instance spins up it creates a new version of itself, and that means it’s difficult to collect data necessary to debug and fix a serverless function.

Third-party tools that log serverless function events exist, but without adding an additional tool, debugging a serverless function can be cumbersome.

## Vendor lock-in

Allowing a vendor to provide all backend services for an application inevitably increases reliance on that vendor. Setting up a serverless architecture with one vendor can make it difficult to switch vendors if necessary, especially since each vendor offers slightly different features and workflows.

## Loss of control

When we choose serverless computing, we don't manage the server. Thus, we lose control of the server hardware, execution environments and updates.

# Links reffered

1. https://www.oreilly.com/library/view/what-is-serverless/9781491984178/ch04.html
2. https://www.bmc.com/blogs/serverless-computing/
3. https://www.cloudflare.com/en-gb/learning/serverless/why-use-serverless/
4. https://www.techrepublic.com/article/serverless-computing-pros-and-cons-5-benefits-and-3-drawbacks/
5. https://brainhub.eu/library/disadvantages-of-serverless-computing#disadvantages-of-serverless-computing-why-it-might-not-work-in-your-case
