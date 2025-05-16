
How much data your publisher program will send to the message broker in one run? 

    - the program will send 5 messege to the maessafe broker. each message will contain a user id and a user name. the data sent is the sum of the serialized size of the 5 messades. 


The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?

    - amqp:// — protocol (Advanced Message Queuing Protocol)

    - guest:guest — username and password (default RabbitMQ credentials)

    - localhost — the broker is running on the same machine as the program

    - 5672 — the default port for AMQP
Running RabbitMQ as message broker.
![image](https://github.com/user-attachments/assets/1290dc82-fd89-47b8-8c37-9c78b1531a04)

Sending and processing event
![image](https://github.com/user-attachments/assets/cdb89054-cbcb-4934-8a2b-bd79dc310556)

The subscriber establishes a connection with the RabbitMQ message broker, confirming active listening. The publisher executes cargo run, sending five messages to the broker. The subscriber processes each message in real-time, demonstrating successful communication. This interaction validates the working message queue system using RabbitMQ and Rust for event-driven communication.


Monitoring chart based on publisher
![image](https://github.com/user-attachments/assets/a2498768-b6e8-4fb3-927d-d7f986bf492a)

The publisher program sends messages to RabbitMQ, causing a spike in the message rate graph. This indicates the number of messages published per second. Despite a queue showing 0 messages, the purple line indicates message acknowledgments, confirming the message flow between the publisher and RabbitMQ broker.

