# Reading 26

## Android Fundamentals

What is an Intent in Android Studios? Give some fresh examples of when you might use it.

`Intent` in Android is a messaging object that you can user to request an action from another app component. There are a lot of things and purposes you can use an `intent`. 

* Starting an activity - starting up an activity in the same  or different app
* Staring a service - background tasks
* Deliver a broadcast - broadcasts are messages that any app can recieve, for system wide announcements

A fresh example:
Suppose you made a photo editing application and wanted users to be able to share an edited image straight to other apps. You can use a share menu with the image attached to start this activity of sharing data/images to other apps.

Describe an Activity in your own word.

An Activity is like a chapter in a book. Each chapter provides a unique part of the story, and as readers progress, they transition from one chapter to another. While each chapter stands on its own and has its own content (UI and data), it's part of a larger narrative (the app). Just as a reader can bookmark a page, return to a previous chapter, or skip ahead, an Activity has various stages in its lifecycle that allow users to enter, leave, and return to specific parts of the app.

## Things I want to know more about

## References

[Android Fundamentals Guide](https://developer.android.com/guide/components/fundamentals)
