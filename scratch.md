Your team is developing a C# application that manages containers in an Azure Storage account by using the Azure.Storage.Blobs .NET client library.

The application must follow security policy that prohibits storing secrets such as connection strings or account keys in code.

You need to authenticate by using Microsoft Entra ID and create a client that can list, create, and delete containers at the account level.

Which two actions should you perform? Each correct answer presents part of the solution. Choose two.

Select all answers that apply.

Instantiate a BlobContainerClient.

Create a BlobClient from the account URL.

Instantiate a BlobServiceClient with the account URL and DefaultAzureCredential.

Assign the Entra ID identity of the application an Azure RBAC role that grants access to blob data.

Enable anonymous public read access on the container so authentication is not required.