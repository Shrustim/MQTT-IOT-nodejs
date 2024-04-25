# MQTT-IOT-nodejs

https://www.youtube.com/watch?v=I8zROK4S2bE
https://explore.skillbuilder.aws/learn/course/external/view/elearning/402/internet-of-things-foundation-series

https://explore.skillbuilder.aws/
https://explore.skillbuilder.aws/learn/mycourses	
https://www.youtube.com/watch?v=qAe2zYqvQTQ

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

