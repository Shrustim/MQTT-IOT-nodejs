# MQTT-IOT-nodejs

https://www.youtube.com/watch?v=I8zROK4S2bE
https://explore.skillbuilder.aws/learn/course/external/view/elearning/402/internet-of-things-foundation-series

https://explore.skillbuilder.aws/
https://explore.skillbuilder.aws/learn/mycourses	
https://www.youtube.com/watch?v=qAe2zYqvQTQ

There are several ways to pass data from an IoT device to cloud storage. The choice often depends on factors such as the nature of the IoT device, the amount of data, the connectivity options available, and the requirements of the application. Here's a list of common methods:
Direct MQTT/AMQP Communication: MQTT (Message Queuing Telemetry Transport) and AMQP (Advanced Message Queuing Protocol) are lightweight and efficient messaging protocols commonly used in IoT. Devices can publish data to a broker, which then forwards the data to cloud storage.
HTTP/HTTPS: IoT devices can send data to cloud storage via HTTP or HTTPS protocols. This method is straightforward and commonly used when devices have internet connectivity and can communicate over standard web protocols.
CoAP (Constrained Application Protocol): CoAP is a lightweight protocol designed for IoT devices with limited resources. It's similar to HTTP but optimized for constrained environments. Devices can use CoAP to communicate with cloud servers.
Message Queueing Systems (e.g., RabbitMQ, Kafka): Message queuing systems can act as intermediaries between IoT devices and cloud storage. Devices send data to a message queue, and cloud applications consume the data from the queue.
Edge Computing: In edge computing architectures, IoT devices process and analyze data locally before forwarding relevant data to the cloud. This reduces latency and bandwidth requirements while still enabling cloud storage integration for long-term storage and analysis.
WebSockets: WebSockets provide full-duplex communication channels over a single TCP connection. IoT devices can establish WebSocket connections with cloud servers to send data in real-time.
Protocol Gateways: If IoT devices use proprietary protocols, protocol gateways can translate these protocols into standard formats (e.g., MQTT, HTTP) understood by cloud services.
File Transfer (FTP, SFTP): For scenarios where IoT devices generate large files or batches of data, file transfer protocols like FTP (File Transfer Protocol) or SFTP (SSH File Transfer Protocol) can be used to upload data to cloud storage.
Direct Database Connection: IoT devices can directly connect to cloud-hosted databases (e.g., SQL databases, NoSQL databases) and insert data into designated tables or collections.
LoRaWAN/Cellular Gateway: In scenarios where IoT devices operate in remote areas or have limited internet connectivity, gateways equipped with long-range communication technologies (e.g., LoRaWAN) or cellular connectivity can collect data from devices and forward it to cloud storage.
Batch Processing: IoT devices can collect and buffer data locally and then periodically upload batches of data to cloud storage. This approach conserves bandwidth and reduces the frequency of data transmission.



IOT

1.Create AWS account 
2.create IAM role of IOT full access
3.Create  certificate in IOT 
4.Create policy in IOT and attach it to above certificate 
5.install aws cli
6.create New user account to configure AWS Cli

https://www.youtube.com/watch?v=u0JyzUGzvJA
https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
commands
aws  configure 
aws --region us-east-1 iot-data publish  --topic "myTopic" --cli-binary-format raw-in-base64-out --payload "{\"uptime\":123,\"temp\":44,\"humidity\":34}"
7.Install MQTT.fx tool for testing
https://web.archive.org/web/20210514230412/https://www.jensd.de/apps/mqttfx/1.7.1/
Message Queue Telemetry Transport Protocol (MQTT)

7.For store data into dynamodb 
-Create rule in IOT core select that topic and dynamod2 version 2
-Create table in dynamo db to store data 
-Create role while creating rule 
-Testing that topic,  pass data to store in dynamodb

8.study related to dynamodb
https://www.youtube.com/playlist?list=PLIRAZAlr4cfZ9tonqGA5zWxtq6MrbSB3O
9.install Nosql workbench and connect AWS dynamo db from laptop 
10.create api using dynamodb and node express sample

