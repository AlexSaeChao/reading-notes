# Reading 37

## Introduction to Amazon S3

What is Amazon S3?

Cloud storage from AWS that is highly scalable and versatile. It is designed to store and retrieve data from anywhere on the web.

List at least 3 features that it offers to its users.

1. Storage management
2. Access management and security
3. Storage logging and monitoring

What is an object key?

In Amazon S3, an object key is a unique identifier for an object within a bucket. It acts as a path or name for the object and is used similarly to a hash map. They are used to retrieve, store and organize in those buckets.

## S3 with Amplify

Which dependencies are needed to install Amplify AWS S3 to your Android application?

We will need Amplify CLI and it's library:

```
dependencies {
    implementation 'com.amplifyframework:aws-storage-s3:2.12.0'
    implementation 'com.amplifyframework:aws-auth-cognito:2.12.0'
}
```

What is needed in order to upload data to your bucket?

You need to initialize the Amplify Framework in the Android application your building. Then configure Amplify with your AWS credentials. Then with Amplify CLI you can add the storage category. Then upload the data or objects to the buckets with the specific key.

``` java
private void uploadFile() {
    File exampleFile = new File(getApplicationContext().getFilesDir(), "ExampleKey");

    try {
        BufferedWriter writer = new BufferedWriter(new FileWriter(exampleFile));
        writer.append("Example file contents");
        writer.close();
    } catch (Exception exception) {
        Log.e("MyAmplifyApp", "Upload failed", exception);
    }

    Amplify.Storage.uploadFile(
            "ExampleKey",
            exampleFile,
            result -> Log.i("MyAmplifyApp", "Successfully uploaded: " + result.getKey()),
            storageFailure -> Log.e("MyAmplifyApp", "Upload failed", storageFailure)
    );
}
```

> Upon successfully executing this code, you should see a new folder in your bucket, called public. It should contain a file called ExampleKey, whose contents is Example file contents.

what method(s) initialize(s) the Amplify Auth and Storage categories?

Initialize Auth:

``` java
Amplify.addPlugin(new AWSCognitoAuthPlugin());
Amplify.configure(getApplicationContext());
```

Initialize Storage:

``` java
Amplify.addPlugin(new AWSS3StoragePlugin());
Amplify.configure(getApplicationContext());
```

## Things I want to know more about

## References

[Introduction to Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/dev/Introduction.html)

[S3 with Amplify](https://docs.amplify.aws/lib/storage/getting-started/q/platform/android/)
