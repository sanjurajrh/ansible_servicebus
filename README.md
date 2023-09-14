# ansible_servicebus
Azure Service Bus is an enterprise integration message broker. Service bus supports two types of communication: queues and topics.
Queues support asynchronous communications between applications. An app sends message to a queue, which stores the messages. The receiving application then connects to and reads the messages from the queue. 
Topics support the publish-subscribe pattern to enable a one-to-many relationship between the message originator and the message receiver(s)

Pre-requisites
=================
1. Azure Subscription account. I have used the free account for this testing
2. Virtual machine/system with Ansible installed and configured to connect to Azure environment
3. We donot have any Ansible Service bus already created. We are not using any existing applications to test
4. Assign the required roles of Ansible Service Bus Data Owner, Azure Service Bus Data Sender and Azure Servuce Bus Data Receiver. To assign this to the user, the organization needs Azure AD Premium P1 or P2.
5. Collection: azure.azcollection
6. Environment used is a local system with ansible installed.
7. The AAP is using the azure credential stored as Credentials in Ansible Controller.


Order of execution
===================
1. Create the Service Bus queue (servicebus_queue.yml)
2. Create the SAS policy (servicebus_queue_policy.yml)
3. Create the Service Bus topic (servicebus_topic.yml)
4. Create the subscription (servicebus_subscription.yml)
5. Create the SAS policy (servicebus_topic_policy.yml)







