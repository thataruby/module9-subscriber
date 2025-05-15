# Advanced Programming Module 9 - Subscriber
### Athazahra Nabila Ruby - 2306173113

> What is `amqp`?
 
AMQP (Advanced Message Queuing Protocol) is a network communication protocol like HTTP/HTTPS that is used for sending messages between applications or services. AMQP allows systems to communicate with each other by sending data over the internet as a stream of bytes.

AMQP supports both point-to-point message delivery and the publisher-subscriber model. In the publisher-subscriber model, one system (the publisher) sends messages that are then forwarded to one or more other systems (subscribers) via a queue. In this tutorial, AMQP is implemented using the crosstown_bus library so that UserCreatedHandler can receive messages sent to the user_created queue.

> What does it mean `guest:guest@localhost:5672` , what is the first guest, and what is the second guest, and what is `localhost:5672` is for?
 
The URI guest:guest@localhost:5672 is used to connect to the AMQP server by including authentication information and the destination address.

- guest (before :) = the username, which is the identity used to log in to the server.
- guest (after :) = the password corresponding to the username. In this URI, it is the same because both username and password use the default value guest.
- localhost = indicates the connection is made to the local machine.
- 5672 = the default port used by the AMQP server.

This URI indicates that the client will establish a connection to a server running on the local machine through port 5672, using the default guest as both the username and password.