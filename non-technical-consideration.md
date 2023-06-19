# Non technical considerations

## Business

### Cost

#### Total cost of ownership

When comparing the cost it doesn't only include the cost incurred for infrastructure but also all the factor like development cost and also include maintenance cost. Following are the main points that are included-

1. DevOps salary
2. SaaS(Software as a Service) bills like monitoring tools.
3. Development or Maintainance efforts (Upgrade, Update, Scaling)

#### Solving right problem

Each server & serverless are used to solve the right problem, cost can be optimized. Tests conducted by UC berkley states that serverless is anti pattern in software development and stigmatizes the distributed computing, hardware accelerated software innovation. To support their study they used AWS lambda & AWS EC2 to train the model. The result was that lambda was 21x slower 7.3x times expensive. Here opting for server than server for data intensive workload.

Serverless is better choice when your software is not compute intensive. Serverless can be choice when you want to delegate the responsibilities of devops to developer thant to hire some separate developer.

Server can be choice in case you want to delegate the hardshiop of managing the server as well as freeing up developer so that they can focus on development of product. But if developer can take up responsibility of handling serverless parameters which are very less compared to server then serverless is better choice.

There are price calculator available which given you requirement can calculate the cost which can help make better decision.

### Security

Cloud provider like AWS manages OS & platform vulnerabilities. But in case of Serveless you don't have access to server & you can't use the security measure IDS (Intrusion Detection System) or IPS (Intrusion Protection System). In case of server architecture, entire server is managed by us in which we can make sure that all the security measures are implemented.

Developing & running the serverless application depends on cloud provider standards. Many of the serverless application can be deployed on single server. Since they are sharing the single machine resources can also create security concerns.

Serverless applications are stateless, and the use of microservices in their architecture exposes the moving parts of the independent functions to authentication failure. For instance, if just one function’s authentication is mishandled in an application with hundreds of serverless functions, it will impact the rest of the application.

### geographical

In both cases of sever & serverless we have option where it can be deployed. This we can leverage to reduce the latency & improve performance.

But when deploying server you need to take care of networking, managing traffic acorss multiple location. This is not case in case of serverless.

When deploying the server across the multiple region, scaling becomes hard in case of server but it is taken care by cloud provider.

## Other factor

### Labour

Based on what you choose server & serverless, labour required for managing the infrastructure can change. If you choose the serverless then people required to manage the infrastructure is less. But if application is deployed on server then people required to manage the infrastructure is also more. If servereless is the choice many of things are already managed remaining few things can be taken care by developers. In case of server there are many things that need to be taken care of which hinders with speed of development if given to devlopers.

With increased labour comes the salaries that need to be paid to the labour. Salary of devops engineer in India is around 7 lakh for opening position. For senior devops it is 13-15 lakh & for lead it is 17-20 lakh.

### Vendor Lock-in

It is condition in which, organisation is stuck with one cloud vendor. Even if they want to migrate to some other it can be hard because of following reasons

- Financial pressure
- Insufficient workforce
- Avoid interruptions to business
- Customer is locked in to inferior product

iTunes is goode exampole of vendor lock-in.

In terms of both server & serverless, both are implemented in different ways by different cloud vendors. If you want to migrate your appication to some other vendor then it is hard.

Vendor lock-in can impact when

- Decline in quality of service
- Vendor changing the product offering
- Vendor going out of business
- Change in pricing

# References

[Is serverless cheaper for your use case? Find out with this calculator.](https://medium.com/serverless-transformation/is-serverless-cheaper-for-your-use-case-find-out-with-this-calculator-2f8a52fc6a68)

[You are thinking about serverless costs all wrong](https://theburningmonk.com/2019/01/you-are-thinking-about-serverless-costs-all-wrong/)

[Vendor Lock in by cloudflare](https://www.cloudflare.com/en-gb/learning/cloud/what-is-vendor-lock-in/)
