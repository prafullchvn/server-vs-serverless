# Technical Considerations

## 1. Scaling

> **Server** <br>
> Resource scaling is a bit of a challenge in server architecture. We need to know how much resource it would take before hand. If a specified amount of resource is allocated it will still be available even if that resource is not in use. Which increases the cost of infrastructure.
> A dedicated person (developer) has to explicitly add or remove resources.
> To solve this problem autoscaling can be used but in autoscaling we need to mention the threashold.
> Which also requires setup and maintenence.
> Additionally the new instances take time to come up.

> **Serverless** <br>
> Serverless computing is known for offering scalable solutions and providing on-demand resources. Scaling is completely automatic and managed by the serverce provider.
> Since the compute container are ephemeral, the service provider handles all the underlying resource provisioning and allocation. We need not to manage VM or cluster.
> One of the benefits this brings is cost saving. Since autoscaling will be taken care by service provider **you will only have to pay for the compute that you need**.

## 2. Latency

Latency is the time taken by the server to respond to a request.

> **Server**<br/>
> In traditional server architecture, there are dedicated servers that receive and process client requests. Most common latency problem we have in this architecture include network latency, computation latency. For example your application logic has authentication and authorization logic which takes time for the request to process and respond to the user.

> **Serverless**<br/>
> In serverless architecture all the latency problems with server architecture are included, because at the end application will still be running on some server just the management of the server is abstracted by the service provider. On top of these there are some factors which increases the latency in the serverless architecture.\
> **1. Startup Latency**\
> Since service provider takes care of scaling, they get the instance down of a particular serverless function after a specified amount of time. When a request comes to the serveless function the provider initializes a new instance of that particular serverless function this is called as **cold start**\
> This Cold-start introduces latency in serveless architecture. This depends on many factors:
>
> - The language in use :- \
>   If you are using interpreted language it would take less time to start the function than a compiled language.
> - Number of libraries in use :- \
>   The more the libraries your function uses the more the time it takes to load them and start the function
> - Whether you need to connect to a VPC :- \
>    For example you are using AWS as your cloud provider and you need VPC, then AWS needs to allocate an ENI (Elastic Network Interface) at container instantiation time.
>
> All the above factors are in controll of developer. So the latency in these factors can be reduced.
>
> **2. State management** <br/>
> Since servelss functions are stateless, the state has to be stored or cached somewhere (depending on the use) like redis or any other mechanism. This increases latency a bit since the state has to be fetched from storage or caching mechanism.

## 3. Resources

## References

> **Server**<br/>
> In order to allocate resources we need to specify the memory, cpu, storage before hand. If the allocated resource are more than required then it is waste of resources, and if they are less then additional resources has to be added.\
> In Cloud computing, the cloud provider takes care of most of the thing, but if specified resources are not enough then we again have to give new specifications for the resources and cloud provider provides those many resources.
>
> **Serveless**<br/>
> In serverless architecture resource allocation like memory, cpu, storage are taken care by the service provider.

1. https://nordicapis.com/server-vs-serverless-benefits-and-downsides/
2. https://martinfowler.com/articles/serverless.html
