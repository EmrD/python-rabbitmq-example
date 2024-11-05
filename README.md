# Python RabbitMQ Example

This is an example repository that sends and tracks the messages using RabbitMQ with Python.

## Installation

To test locally, follow these steps; 

- Installing RabbitMQ
``sudo apt update |sudo apt upgrade -y | sudo apt install -y erlang | echo "deb https://dl.bintray.com/rabbitmq/debian buster main" | sudo tee /etc/apt/sources.listd/rabbitmq.list | wget -O- https://dl.bintray.com/rabbitmq/DEB-GPG-KEY.rpm | sudo apt-key add - | sudo apt update | sudo apt install -y rabbitmq-server``

- Start RabbitMQ
`sudo systemctl start rabbitmq-server` or `sudo service rabbitmq-server start`

- Enable RabbitMQ Web Management
`sudo rabbitmq-plugins enable rabbitmq_management`

- Enter RabbitMQ Web Interface
`http://localhost:15672`

- Username and password is ``guest`` as default. 

## Send And Receive Messages With Python

``server.py`` is receiving messages. 
``client.py`` is sending messages. 