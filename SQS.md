## Definition
- just a queue of messages and the client sides (who have access to it) could do continuously pull to get the updated


## Use Cases

**Asynchronous workflows** : SQS can be used to facilitate asynchronous processing between application components. A message sent to an SQS queue can trigger an event in another part of an application, even if that other part of the application is not running at the same time.

**Decoupling services** : By introducing a messaging layer between two parts of an application, it allows those parts to be developed, deployed, and scaled separately. This can also reduce dependency problems when deploying changes to an existing system.

**Message buffering** : in certain scenarios, such as when dealing with many small requests or burst traffic, it can be helpful to buffer requests into a queue before they are processed. This can easily be done with SQS.

**Workload balancing** : Requests from different users can be added to a single queue and processed in parallel by multiple consumers. This enables load balancing across a system.


## SQS vs. SNS
The primary difference between these two services is that while SQS is a pull-based system that requires applications to poll a queue to receive messages, SNS works by sending messages to subscribed applications and devices without requiring them to poll or query a message queue.


## Advantages
1- you decide when to recieve the data (you decide when to pull the data)


2- prevent you from losing the data unlike SNS if the client didnt recieve the message it will be lost


## Disadvantages
Limited Durability: While SQS offers durability options, it only retains messages for 14 days. Depending on your requirements, this may not be long enough.
Message Size Limit: The maximum size of an SQS message is 256KB. If you need messages larger than this you will need to look into other solutions.
Latency: SQS is not always the fastest option when it comes to sending a receiving data due to its asynchronous nature.
