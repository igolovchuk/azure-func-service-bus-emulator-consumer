# Introduction
Extended version of Azure Service Bus Emulator [example](https://github.com/piotr-rojek/devopsifyme-sbemulator/tree/main/src/Example.AzureFunction) accomodated to Mac M1 usage.

# Getting Started
TODO: Guide users through getting your code up and running on their own system. In this section you can talk about:
1.	Install cacert.cer (MacOS - under System keychain), use ```sudo docker cp {emulator-containerId}:/app/cacert.cer cacert.cer``` to grab the .cer file.
2.	Install cert.pfx, password: password (MacOS - under System keychain), use ```sudo docker cp {emulator-containerId}:/app/cert.pfx cert.pfx``` to grab the .pfx file.
3.	Run in the terminal: ```docker compose up -d``` , under the project root
4.	Run the application in debug node
5.  Open [RabbitMQ UI](http://localhost:15672/), topics and subscription should be automatically created.
6.  Open topic(exchange), and try to publish the message from the payload using topic as routing key.
7.  Run ```docker compose stop``` in order to shut down the emulator.

# References
- [Simple Azure Service Bus Emulator](https://devopsifyme.com/simple-azure-service-bus-emulator-finally-here/)
- [SB Emulator Github](https://github.com/piotr-rojek/devopsifyme-sbemulator)
