A background worker initializes a new environment for an existing Azure Cosmos DB for NoSQL database named telemetry. The environment may or may not have the required container.

Initialization must be idempotent so that repeated runs do not throw errors.

You need to create a container named logs with partition key path /deviceId by using code.

Which method should you call?

Select only one answer.

database.GetContainer("logs").ReadContainerAsync()

database.CreateContainerAsync(id: "logs", partitionKeyPath: "/deviceId")

database.CreateContainerIfNotExistsAsync(id: "logs", partitionKeyPath: "/deviceId")

CosmosClient.CreateContainerIfNotExistsAsync(id: "logs", partitionKeyPath: "/deviceId")