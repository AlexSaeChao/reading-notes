# Authentication

This section covers the basics of authentication and authorization. Authentication verifies a user's identity, while authorization determines what they can access. OAuth is a framework that allows users to grant access to their resources on one website to another without sharing login credentials. It works through different flows such as the Authorization Code Flow, Implicit Flow, Client Credentials Flow, etc., each serving specific purposes and security considerations. We also mentioned OpenID, which works alongside OAuth for identity verification using credentials from other websites.

## What is OAuth

What is OAuth?

> OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

Give an example of what using OAuth would look like.

> The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

How does OAuth work? What are the steps that it takes to authenticate the user?

1. User initiates the process
2. Request token
3. User grants permission
4. Redirect back to the website or application
5. Access token exchange
6. Access protected resources

What is OpenID?

OpenID is a way for users to prove who they are when using a website or app by using their existing login information from another website. It works together with OAuth, which is about granting access to resources. So, while OAuth decides what you can access, OpenID verifies your identity.

## Authorization and Authentication flows

What is the difference between authorization and authentication?

Authentication is the process of verifying the identity of a user or entity. It ensures that the user is who they claim to be. Authorization is the process of granting or denying access to specific resources or actions based on the authenticated user's permissions.

What is Authorization Code Flow?

> Because regular web apps are server-side apps where the source code is not publicly exposed, they can use the Authorization Code Flow, which exchanges an Authorization Code for a token.

This flow is used when a confidential client (a server-side application) wants to obtain an access token on behalf of a user. The user is redirected to an authorization server, where they authenticate and provide consent. Upon successful authentication and consent, an authorization code is returned to the client, which then exchanges the code for an access token.

What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

This is similar to the Authorization Code Flow but adds an extra layer of security. It is used by apps that run on devices like smartphones.

What is Implicit Flow with Form Post?

This flow is for apps that run in web browsers. Instead of exchanging an authorization code, the access token is sent directly to the app in the form of a response to a form submission.

What is Client Credentials Flow?

This flow is for apps that need to access resources on their own without user involvement. The app exchanges its own credentials (like a secret key) for an access token to access the protected resources.

What is Device Authorization Flow?

his flow is for devices that can't directly enter login credentials, like smart TVs. The user authorizes the device using a different device, like a smartphone or computer, by entering a verification code displayed on the device.

What is Resource Owner Password Flow?

This flow allows users to directly provide their username and password to an app. The app exchanges these credentials for an access token to access the user's data. This flow should be used cautiously and only when necessary, as it involves the app handling the user's sensitive credentials.

## Things I want to know more about

In what use cases do the authorization code flow wittht the PKCE instead of the regular one?

## References

[What is OAuth? How the open authorization framework works](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

[Authentication and Authorization Flows](https://auth0.com/docs/get-started/authentication-and-authorization-flow)
