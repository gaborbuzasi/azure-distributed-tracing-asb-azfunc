# Application Insights Distributed Tracing

### This is a proof of concept to test how correlated application insights telemetry works in a distributed environment.

## Components: 

- Azure Service Bus + queue/topic
- Azure Function with HTTP trigger sending messages to an Azure Service Bus queue/topic
- Azure Function with Azure Service Bus trigger to read messages from the queue

## To Deploy:

#### Requirements:
- Azure account
- Azure CLI installed

In a command shell or PowerShell type:

```
az deployment sub create --name <name of deployment> --location northeurope --template-file <path-to-arm-template> --parameters <path-to-arm-template-param> --verbose
```

This will initiate a subscription level deployment with the resources defined in the ARM template.