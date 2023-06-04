# About server and serverless

## Server
A server is a software or hardware device that accepts and responds to requests made over a network. On the Internet, the term "server" commonly refers to the computer system that receives requests for a web files and sends those files to the client.

### What are they used for?
Servers manage network resources. For example, a user may set up a server to control access to a network, send/receive e-mail, manage print jobs, or host a website.

Servers are also proficient at performing intense calculations. Some servers are committed to a specific task or one website, often called dedicated servers. However, many servers today are shared servers that take on the responsibility of e-mail, DNS, FTP, and multiple websites in the case of a web server.

## Serverless
The term serverless is misleading because servers still exist, but developers do not need to worry about managing the server. Going serverless means that developers focus on the application at the task level instead of at the server level. Now, they don’t need to worry about managing and operating servers or runtimes in the cloud or on-prem.

Serverless can also be described as [Functions as a Service (FaaS)](#faas). FaaS products execute functions (code) that are run on demand in response to events. The benefit to running code on demand is in the use case where your code does not need to be running full time.

This sounds a little like microservices, and the concept is similar. The goal of a microservice is to break our large application into small, decoupled, independent systems that connect back together to make our application work. Functions go one step further and are smaller than microservices, think one microservice can contain multiple functions. The difference comes in use cases. There are some things that are not suitable for functions and vice versa.

## FaaS
Serverless and Functions-as-a-Service (FaaS) are often conflated with one another but the truth is that FaaS is actually a subset of serverless.

FaaS is the most central technology in serverless architectures, is focused on the event-driven computing paradigm wherein application code, or containers, only run in response to events or requests.

Serverless is focused on any service category, be it compute, storage, database, messaging, api gateways, etc. where configuration, management, and billing of servers are invisible to the end user.

There are other services similar to FaaS - SaaS, PasS.

# Links Reffered
1. https://www.computerhope.com/jargon/s/server.htm
2. https://www.ibm.com/topics/faas#:~:text=the%20next%20step-,What%20is%20FaaS%3F,building%20and%20launching%20microservices%20applications.
3. https://www.xtivia.com/blog/compare-faas-paas-saas/ 
