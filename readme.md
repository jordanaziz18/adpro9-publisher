
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

