# Reflection Module 9: Subscriber
## a. what is amqp?
AMQP, or Advanced Message Queuing Protocol, is an open standard protocol designed for message-oriented middleware, ensuring reliable and secure communication across heterogeneous networks. It enables interoperable messaging between distributed applications, managing complex tasks such as message queuing, routing, and security. AMQP is particularly valuable in event-driven and microservices architectures where components need to communicate asynchronously across multiple servers or locations, promoting robust, loosely coupled system designs.

## b. what it means? guest:guest@localhost:5672 , what is the first quest, and what is the second guest, and what is localhost:5672 is for?
string `amqp://guest:guest@localhost5672` specifies the connection details for amqp server. here is how each component of the string funcitons:
1. `guest`: this is the username required for server login. it's used for authenticating the user attempting to connect to the amqp server
2. `guest`: following the colon after the first `guest`, the second guest is the password linked witht he username. the password is required to authenticate the connection
3. `localhost`: indicates the hostname or ip address of the server.
4. `5672`: is the port number where the server listens for incoming connection. it's the default port for amqp connections that do no tuse TLS/SSL

The chart below shows that the simulation of the slow response creates a queue for the system
![alt text](images/image4.png)

The chart shows the response of the load handled by the subscriber app handlling 5 consecutive cargo run from publisher
![alt text](images/image5.png)