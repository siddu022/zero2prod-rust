## we expect Cloud-native applications:
- to be scalable [scalable means that the application can handle more requests by adding more resources]
- to be resilient [resilient means that the application can handle failures]
- to be observable [observable means that the application can be monitored]
- to be secure [secure means that the application is protected from unauthorized access]
- to be automated [automated means that the application can be managed without human intervention]
- to be portable [portable means that the application can run on any cloud provider]
- to be cost-effective [cost-effective means that the application is optimized for cost]
- to be fast [fast means that the application can respond quickly to requests]
- to be efficient [efficient means that the application can handle requests with minimal resources]
- to be maintainable [maintainable means that the application can be easily updated]

1. To achieve high-avaiablity while running in fault-prone environments, cloud-native applications should be designed to be resilient.
2. To achieve us to continuously release new versions with zero downtime.
3. To handle dynamic workloads, cloud-native applications should be designed to be scalable.

High availability implies that our application should be able to serve requests with no downtime even if one or more of our machines suddenly starts failing (common occurrence in cloud environments). This forces our application to be distributed across multiple machines, which in turn makes it more resilient to failures.


