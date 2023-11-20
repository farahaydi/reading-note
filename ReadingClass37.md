# What is Amazon S3?

Amazon S3, or Simple Storage Service, is a cloud storage service by Amazon Web Services. 
It lets you store and retrieve any amount of data securely over the internet. Key features include scalability, high durability, security controls, and different storage options based on your needs.
It's commonly used for data backup, websites, mobile apps, and more in the AWS cloud.

# List at least 3 features that it offers to its users.
Scalability: Amazon S3 provides virtually unlimited storage capacity, allowing users to scale their storage needs easily as their data grows.

Durability: With 99.999999999% (11 9's) durability, Amazon S3 ensures high reliability and protection against data loss due to hardware failures.

Security Controls: Users can implement access control lists (ACLs), bucket policies, and integrate with AWS Identity and Access Management (IAM) to control and secure access to their stored data.
# What is an object key?
In Amazon S3, an object key is a unique identifier assigned to each object (file) stored within a bucket. The combination of the bucket name and the object key forms the unique identifier for that specific object. The object key is essentially the path or name of the object within the bucket.

For example, in the URL https://s3.amazonaws.com/my-bucket/my-folder/my-file.txt:

"my-bucket" is the bucket name.
"my-folder/my-file.txt" is the object key.
Object keys are case-sensitive and can include slashes ("/") to create a folder-like structure within a bucket. The object key, along with the bucket name, is used to address and retrieve specific objects from Amazon S3.

# Which dependencies are needed to install Amplify AWS S3 to your ndroid application?
To use Amplify AWS S3 in your Android app, add these dependencies in your build.gradle:

dependencies {
implementation 'com.amplifyframework:aws-storage-s3:2.14.5'
implementation 'com.amplifyframework:aws-auth-cognito:2.14.5'
}
These enable interactions with Amazon S3 storage and provide authentication through AWS Cognito.

# What is needed in order to upload data to your bucket?

To upload data to your bucket using Amplify AWS S3:

Set up Amplify Storage in your Android app.
Add Amplify libraries for S3 and authentication in your app's dependencies.
Initialize Amplify with S3 and authentication plugins.
Ensure user authentication or configure guest access.
Use Amplify Storage API to upload data to your bucket.
# what method(s) initialize(s) the Amplify Auth and Storage categories?
Amplify.configure(getApplicationContext());
This method is part of the Amplify library and is used to complete the initialization process after adding plugins for the Auth and Storage categories. It configures the Amplify framework with the provided context, enabling the configured plugins and making the services ready for use.









