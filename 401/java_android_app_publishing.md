# Reading 34

## Publishing apps on the Google Play Store

**How are releases and versioning related?**

In Android development, versioning and releases go hand in hand:

Unique Identification: The version code is like a special ID that helps tell different app versions apart. When we raise the version code with each update, it's a way for both the system and users to know which version is which.

Finding Updates: Android uses the version code to see if there's a new app version available for users. If the new version's code is higher than the one they have, Android knows it's time to offer an update.

Putting It on the Play Store: When we want to share a new app version on the Google Play Store, we give it an updated version code and version name. This helps the Play Store handle updates for people who already use the app and show the version details to new users.

Communication between Users and Developers: Versioning helps users and developers chat about different app versions. Version names make it clear what's new in updates for users, while version codes help developers figure out and fix problems in specific releases.

**What are the 5 main tasks you need to complete to prepare your application for release to the Google Play Store?**

> Preparing your app for release is a multistep process involving the following tasks:

**Configure your app for release.**
> At a minimum, you need to make sure that logging is disabled and removed and that your release variant has debuggable false for Groovy or isDebuggable = false for Kotlin script set. You should also set your app's version information.

**Build and sign a release version of your app.**
> You can use the Gradle build files with the release build type to build and sign a release version of your app. For more information, see Build and run your app.

**Test the release version of your app.**
> Before you distribute your app, you should thoroughly test the release version on at least one target handset device and one target tablet device. Firebase Test Lab is useful for testing across a variety of devices and configurations.

**Update app resources for release.**
> Make sure that all app resources, such as multimedia files and graphics, are updated and included with your app or staged on the proper production servers.

**Prepare remote servers and services that your app depends on.**
> If your app depends on external servers or services, make sure they are secure and production ready.

## Things I want to know more about

## References

[Google’s app publishing guide](https://developer.android.com/studio/publish)
