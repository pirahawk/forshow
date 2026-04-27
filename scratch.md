A .NET API stores multi-tenant order data in Azure Cosmos DB for NoSQL. In some new environments, the database and container may not exist.

Startup must initialize these resources in an idempotent way so that repeated runs do not fail.

You need to create the database and a container with partition key /tenantId and provision 400 request units per second (RU/s) on the container by using code.

Which method should you call?

Select only one answer.

CosmosClient.CreateDatabaseIfNotExistsAsync("appDb", throughput: 400)followed bydatabase.CreateContainerIfNotExistsAsync("orders", "/tenantId")

CosmosClient.CreateDatabaseAsync("appDb")followed bydatabase.CreateContainerAsync("orders", "/tenantId", throughput: 400)

CosmosClient.CreateDatabaseIfNotExistsAsync("appDb")followed bydatabase.CreateContainerIfNotExistsAsync("orders", "/tenantId", throughput: 400)