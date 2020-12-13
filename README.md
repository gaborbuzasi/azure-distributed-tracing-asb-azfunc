# Application Insights Distributed Tracing

### This is a proof of concept to test how correlated application insights telemetry works in a distributed environment.

## Components: 

- Azure Service Bus + queue/topic
- Azure Function with HTTP trigger sending messages to an Azure Service Bus queue/topic
- Azure Function with Azure Service Bus trigger to read messages from the queue