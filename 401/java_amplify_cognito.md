# Reading 36

## Amplify Cognito

Where in your application should you check the current auth session?

In any pages where you display PII, accessing sensitive information or allowing users to perform actions that require auth. You can check the authentication session using Amplify's Auth module.

what is the command that is used to push your changes to the cloud?

Using the Amplify CLI to push to the cloud:

``` script
amplify push
```

What does Amplify Auth do for your application?

Amplify Auth can help me with User Registration and sign-up, User Auth and sign-in, other social sign-ins, Password management, and Token management to AWS Resources.  

## Things I want to know more about

So with additions to users we would add a users model and push that to DynamoDB?

## References

[Amplify and Cognito (read “Getting started” and “Sign in” subsections)](https://docs.amplify.aws/lib/auth/getting-started/q/platform/android/)