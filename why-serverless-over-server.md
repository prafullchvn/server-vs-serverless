# When to use server-less over server

  - Building applications with serverless functions requires a different approach than traditional server hosting, and the decision to use serverless depends on the problem it solves and the time investment required.

  - Serverless is advantageous for scaling to large amounts of traffic at a low cost, but learning the nuances and setting up a local development environment can be time-consuming.

  - While the serverless framework provides tools and documentation for managing resources and deployment, the development of functions lacks a standardized framework. Serverless is still evolving, and if you're comfortable with setting up a development environment and using a preferred language, it may be worth waiting for further maturity.

  - If you plan to use a new JavaScript framework for the frontend and host API endpoints with serverless, it can be relatively straightforward to figure out. However, if you anticipate more complex backend requirements, be prepared for a significant time investment.

  - Consider going the serverless route when decreasing go-to-market time is a critical factor. Serverless architectures are ideal for building lightweight, flexible applications that can be quickly expanded, upscaled, or updated.

  - Serverless is well-suited for projects with fluctuating usage and high computing power requirements in short bursts. Applications like data integration pipelines or machine learning model training can benefit from cost reductions by going serverless.

  - Serverless is a natural fit for stateless processes such as email senders or push notification agents. These processes involve short-running logic, have high-performance requirements, and don't rely on persistent state or direct access to a filesystem.

## Applications (Examples)
s
  - [AWS Lambda](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)
  - [Microsoft Azure functions](https://azure.microsoft.com/en-in/products/functions/?ef_id=_k_CjwKCAjwhJukBhBPEiwAniIcNY9uKqqvOpmtUbCsUS-QHCtA4M5Pih7XOfMzxMPd7KyoPVqazcSpDBoC1nEQAvD_BwE_k_&OCID=AIDcmmf1elj9v5_SEM__k_CjwKCAjwhJukBhBPEiwAniIcNY9uKqqvOpmtUbCsUS-QHCtA4M5Pih7XOfMzxMPd7KyoPVqazcSpDBoC1nEQAvD_BwE_k_&gclid=CjwKCAjwhJukBhBPEiwAniIcNY9uKqqvOpmtUbCsUS-QHCtA4M5Pih7XOfMzxMPd7KyoPVqazcSpDBoC1nEQAvD_BwE)
  - [Google cloud functions](https://cloud.google.com/functions)
  - [IBM OpenWhisk](https://developer.ibm.com/openwhisk/)


#### Tip : 
  Utilizing [MidyJS](https://middy.js.org), a middleware npm package that helps abstract configuration and promotes code reuse between functions.



# References
  - https://www.reddit.com/r/node/comments/8e5n6r/when_to_use_servers_when_to_go_serverless/
  - https://snipcart.com/blog/why-serverless-example
