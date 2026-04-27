An operations team plans to tag a container that has two name–value pairs. After tagging the container, the team must verify the pairs during startup logging by using the Azure Storage .NET client library and a BlobContainerClient for the target container.

You need to update the container metadata and then read it back for logging.

Which two methods should you use? Each correct answer presents part of the solution. Choose two.

Select all answers that apply.

BlobClient.DownloadToAsync

BlobContainerClient.GetBlobsAsync

BlobServiceClient.SetPropertiesAsync

BlobContainerClient.SetMetadataAsync

BlobContainerClient.GetPropertiesAsync