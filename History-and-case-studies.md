# History

Servers have been around since the early days of computing. In the 1960s, mainframe computers were used as servers to store and process data. These early servers were large and expensive, and only large corporations and government agencies could afford to use them.

As technology evolved, servers became smaller and more affordable. In the 1980s, personal computers became popular, and companies began using them as servers for local networks. In the 1990s, the internet became widely available, and servers were used to host websites and provide email services.

The first "pay as you go" code execution platform was Zimki, released in 2006, but it was not commercially successful. In 2008, Google released Google App Engine, which featured metered billing for applications that used a custom Python framework, but could not execute arbitrary code. PiCloud, released in 2010, offered FaaS support for Python. Amazon launched a similar service, Lambda in 2015. Now, developers could create software and not have to worry about hardware, operating system maintenance, scalability, or locality.

Several serverless databases have emerged in the last few years. These systems extend the serverless execution model to the RDBMS, eliminating the need to provision or scale virtualized or physical database hardware. Nutanix offers a solution named Era which turns an existing RDBMS such as Oracle, MariaDB, PostgreSQL or Microsoft SQL Server into a serverless service. Amazon Aurora offers a serverless version of its databases, based on MySQL and PostgreSQL, providing on-demand, auto-scaling configurations.

# Case studies

## 1. Codepen

Codepen has been around since 2012 and has quickly become a standard for web developers. People use it to share pieces of code and examples that help newcomers get a jump start in their development career.
  - Right now Codepen servers up to 200 000 requests per hour and while that is impressive, what surprised me is the fact that all their infrastructure is run by a one-man DevOps team.
  - With serverless, the business can avoid issues that are connected with the production and market readiness, providing improved performance and at the same time, growing the audience.

## 2. Zalora
Zalora is one of the biggest fashion stores in Asia employing around 1500 people with a user base of over 20 million users. They have a cool mission statement: “fashion on-demand, 24/7 at your doorstep”. They rely heavily on AWS and Lambda to make sure every customer gets access to the website and apps without worrying about scaling issues.

> “We outgrew what the server world offered to us and it was the right time for us to switch over to a provider like AWS” - Karthik Subramanian – CTO at Zalora

> "The capabilities that AWS provides to secure our SAP applications are beyond what we could have deployed in an on-premises or private cloud setup.” - Raymond Leong - Director of Enterprise Technology, Zalora Group

Why Zelora is using AWS:
  - Accelerating S/4HANA Deployment
  - Reduced Cost and Effort
  - Security and Compliance
  - Support at Every Stage
  - Real-Time Customer Insights

## 3. Coca-Cola
The Coca-Cola Company migrated to AWS to reduce costs and increase operational efficiencies. Moving to a DevOps model, The Coca-Cola Company leveraged AWS Elastic Beanstalk to enable its creative agencies to more efficiently deploy applications. The company also used AWS Auto Scaling to optimize performance and costs with its applications, allowing them responding better to sudden influxes of site traffic.
- By migrating to AWS, The Coca-Cola Company achieved 40 percent operational savings, coupled with an 80 percent reduction in IT help desk tickets due to added automation.
- By adopting storage, database, compute, and analytics solutions from AWS, Coca-Cola Andina boosted the productivity of its analytics team by 80 percent, facilitating more data-driven decisions to maintain its competitive advantage and increase company revenue.

> "AWS was the cloud solution that would meet all the expectations defined for our data lake." - Luis Valderrama - Chief Technology Officer, Coca-Cola Andina

## 4. Amazon Prime Video
The Amazon Prime Video team’s recent case study has revealed an interesting shift from a serverless microservices architecture to a monolithic approach. This change resulted in a significant 90% reduction in operating expenses.

The Amazon Prime Video case study demonstrates the importance of finding the right balance between serverless and microservices architectures for specific use cases. While serverless computing may offer benefits such as scalability and reduced operational overhead, it may not always be the optimal solution for every application or system. Similarly, microservices can provide increased flexibility, but they may also introduce unnecessary complexity in some situations.

In the case studies, they have stated that their service performed multiple state transitions for every second of the stream, so they quickly reached account limits. Besides that, AWS Step Functions charges users per state transition.

The solution now runs on EC2 (Elastic Compute Cloud) and ECS (Elastic Container Service), with “a lightweight orchestration layer to distribute customer requests.”

The paper concludes that “Microservices and serverless components are tools that do work at high scale, but whether to use them over monolith has to be made on a case-by-case basis. Moving our service to a monolith reduced our infrastructure cost by over 90%. It also increased our scaling capabilities.”


# references
1. [Server History](https://www.linkedin.com/pulse/guide-servers-usage-history-evolution-sanjay-k-mohindroo-/?trk=pulse-article_more-articles_related-content-card)
2. [Serverless wiki for history](https://en.wikipedia.org/wiki/Serverless_computing)
3. [Serverless history](https://dashbird.io/blog/origin-of-serverless/)
4. [Zalora](https://aws.amazon.com/solutions/case-studies/zalora-sap/)
5. [List of companies using serverless 1](https://dashbird.io/blog/companies-using-serverless-in-production/)
6. [List of companies using serverless 2](https://www.techmagic.co/blog/7-top-companies-using-serverless/)
1. [Coca-Cola Data Lake Case Study](https://aws.amazon.com/solutions/case-studies/innovators/coca-cola/)
1. [Coca-Cola migration Case Study](https://aws.amazon.com/solutions/case-studies/coca-cola-migration/)
1. [Amazon prime video 1](https://medium.com/@abhishekranjandev/the-amazon-prime-video-monolith-shift-dissecting-microservices-serverless-and-the-real-world-ec18e429ad6f)
1. [Amazon prime video 2](https://devclass.com/2023/05/05/reduce-costs-by-90-by-moving-from-microservices-to-monolith-amazon-internal-case-study-raises-eyebrows/)

