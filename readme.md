
How much data your publisher program will send to the message broker in one run? 

    - the program will send 5 messege to the maessafe broker. each message will contain a user id and a user name. the data sent is the sum of the serialized size of the 5 messades. 


The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?

    - amqp:// — protocol (Advanced Message Queuing Protocol)

    - guest:guest — username and password (default RabbitMQ credentials)

    - localhost — the broker is running on the same machine as the program

    - 5672 — the default port for AMQP

