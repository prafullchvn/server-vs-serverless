# What is Serverless Edge Computing

### Edge Computing 

  Edge computing is a decentralized computing model that brings computation and data storage closer to the edge of the network, closer to where the data is generated or consumed. In edge computing, data processing occurs near the source of data, rather than sending it to a centralized cloud or data center. This approach reduces latency, conserves network bandwidth, and enables real-time or near-real-time data processing.

### Serverless Edge Computing

  Serverless edge computing combines the principles of serverless computing and edge computing to enable running serverless functions at the edge of the network. It brings the benefits of both paradigms together, allowing for low-latency, event-driven computing closer to the data source.

  In serverless edge computing, the functions are deployed and executed on edge devices, such as edge servers, gateways, or IoT devices, rather than in a centralized cloud. This proximity to the data source reduces the round-trip time and network latency, enabling faster response times and real-time processing.

#### How Serverless Edge Computing works?

  - Deployment: The serverless functions are deployed to edge nodes or devices located at the network edge, closer to where data is generated or consumed. These edge nodes can be geographically distributed, allowing for localized processing.

  - Event-driven execution: When an event occurs, such as a sensor reading, a user request, or a system trigger, the edge node triggers the corresponding serverless function to process the event. The function executes locally, without the need to transmit the data to a centralized cloud.

  - Scalability and resource management: The edge computing infrastructure manages the scalability and resource allocation of the serverless functions at the edge. It ensures that the necessary computing resources are available to handle the workload, whether it's scaling the number of instances or dynamically provisioning resources on-demand.

#### Benefits
  - Low latency: By processing data at the edge, serverless edge computing reduces the round-trip time and network latency, resulting in faster response times and improved user experience.

  - Real-time processing: Serverless functions executed at the edge enable real-time or near-real-time data processing, making it suitable for time-sensitive applications, such as IoT, robotics, or edge AI.

  - Bandwidth optimization: Since data processing occurs locally at the edge, only relevant data or processed results need to be transmitted to the centralized cloud, reducing the bandwidth requirements and associated costs.

  - Offline functionality: Serverless edge computing allows applications to operate even when there is limited or intermittent network connectivity. The functions can continue processing data locally, providing uninterrupted functionality.

  - Enhanced data privacy and security: With serverless edge computing, sensitive data can be processed and analyzed locally, minimizing the need for transmitting data to external cloud servers. This approach enhances privacy and security by reducing the exposure to potential security risks associated with data transmission over the network.

`Serverless edge computing is particularly useful in scenarios where low latency, real-time processing, and localized data processing are critical requirements. It is often employed in edge AI applications, industrial IoT, smart cities, and other use cases where processing data at the edge brings significant advantages.`

###### References
https://www.accenture.com/in-en/insights/cloud/edge-computing-index#:~:text=Edge%20computing%20is%20an%20emerging,led%20results%20in%20real%20time.
https://www.redhat.com/en/topics/edge-computing/what-is-edge-computing?sc_cid=7013a0000034mFIAAY&gclid=Cj0KCQjw7aqkBhDPARIsAKGa0oIRhaVIGDxss9ooaSotdBuO-MDXloI0J1KEhL6ZFUWHSGk7U0gzIp4aAv0oEALw_wcB&gclsrc=aw.ds
https://www.accenture.com/in-en/insights/cloud/edge-computing-index#:~:text=Edge%20computing%20is%20an%20emerging,led%20results%20in%20real%20time.