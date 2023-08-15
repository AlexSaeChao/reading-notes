# Android Fundamentals continued

## Intro

This page explores Android's Shared Preferences and how it's similar to other technologies. We'll discuss the importance of testing and delve into how Android's back stack operates, using a simple analogy. Dive into the resources below to learn more.

## Questions

What is a technology you’ve used before that is similar to Shared Preferences?

Shared Preferences is a mechanism for storing simple key-value pairs of data persistently in Android apps. From what I can remember I have used Node.js and Local Storage.

Why is testing important? Give at least 4 reasons, and explain which is the most important to you and why.

1. Ensuring Correct Functionality - To make sure that the software works as intended and meets the specified requirements. I think it is the important to me at this time because the specifications are truely held as a requirement.

2. Identifying and Fixing Bugs and Issues Early - To find and fix defects before they reach the end-users or production environment. This one kind of goes hand in hand with functionality as we will be squashing bugs if we are testing the if it works correctly.

3. Enhancing User Experience - Through testing, developers can gauge performance issues, UI/UX glitches, or bottlenecks that may frustrate users, getting feedback on what we can improve on while maintaining the specified requirements can really improve the application for the better.

4. Reducing Long-term Costs - Fixing a bug in production is often more expensive than catching it early in a development or staging environment. The costs aren't just financial, releasing buggy software can damage a company's reputation, leading to loss of trust among users or clients.

Create an analogy for Tasks and the back stack. Have we used a similar system before? Explain.

Imagine a dining facility with a spring-loaded plate dispenser. As soldiers take plates for their meals, they pull from the top of the stack. After cleaning, plates are added back to the top of the stack, pushing the others down. If you want to retrieve the plate that was used three meals ago, you'd need to remove the two plates that were added after it. This stack of plates, with its "last on, first off" behavior, mirrors the back stack in Android, where the most recent task (or activity) is the first one you'd return to when navigating backward.

I believe things like nest for/while loops and the nav system for browers function similarly.

## Things I want to know more about

## References

[Android SharedPreferences](https://developer.android.com/training/data-storage/shared-preferences)

[Espresso Testing (read Overview, Basics, and Recipes, plus any others that look interesting)](https://developer.android.com/training/testing/espresso)

[Ridiculous superpower: the Espresso Test Recorder](https://developer.android.com/studio/test/espresso-test-recorder)

[Android Tasks and the Back Stack](https://developer.android.com/guide/components/activities/tasks-and-back-stack)
