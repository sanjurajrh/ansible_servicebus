# ansible_servicebus
Azure Service Bus is an enterprise integration message broker. Service bus supports two types of communication: queues and topics.
Queues support asynchronous communications between applications. An app sends message to a queue, which stores the messages. The receiving application then connects to and reads the messages from the queue. 
Topics support the publish-subscribe pattern to enable a one-to-many relationship between the message originator and the message receiver(s)

Pre-requisites
=================
# Azure subscription account. I have used the free account for this testing
# Virtual machine/system with Ansible installed and configured to connect to Azure environment

Order of execution
===================
1. Create the Service Bus queue (servicebus_queue.yml)
2. Create the SAS policy (servicebus_queue_policy.yml)
3. Create the Service Bus topic (servicebus_topic.yml)
4. Create the subscription (servicebus_subscription.yml)
5. Create the SAS policy (servicebus_topic_policy.yml)







