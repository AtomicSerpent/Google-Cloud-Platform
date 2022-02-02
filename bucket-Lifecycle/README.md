### Setting Cloud Storage Lifecycle Rules

Click the icon in the top navigation to activate Cloud Shell.

In the Cloud Shell, enter the following code:

> gsutil lifecycle get gs://&lt;BUCKET_NAME>

Review the output.

**Set lifecycle rule with JSON file.**
Enter the following to set the lifecycle rules using the JSON file:

> gsutil lifecycle set example.json gs://&lt;BUCKET_NAME>

Verify that the lifecycle rule has been added in the console.
