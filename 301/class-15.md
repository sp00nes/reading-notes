# Class 15 Reading Notes *(11/17/22)*

[*back*](../README.md)

## What is OAuth?

1. An open-standard authorization protocol/framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. A secure, third-party, user-agent, delegated authorization.
2. When you go to a website, and the options to log in or sign up include not only the traditional option of entering your username & password, but also options to login via another website's login (such as logging into a shopping website using your login for google, facebook etc.)
3. Steps
    - first website connects to second website, using 0Auth to verify user's identity
    - second site generates a one-time token & one-time secret uniqe to the transaction and parties involved
    - first site give token and secret to the initiating user's client software
    - client's software presents the request token and secret to their authorization provider (may or may not be second site)
    - client may be asked to authenticate, if not already done with authorization provider. after authentication, client is asked to approve the authorization transaction to the second site
    - user approves a particular transaction type at the first site (or software silently approves it)
    - user is given an approved access token (previously a request token)
    - user gives access token to first site
    - first site gives token to second site as proof of authentication on behalf of the user
    - second site lets first site use it on behalf of the user
    - user sees successfully completed transaction occurring
4. It's for authentication, rather than authorization. Whereas 0Auth is for machines logging into maches on behalf of humans, OpenID is for humans logging into machines. It was supposed to be a single sign-in that users could use to log in to various websites, but that never caught on. Now it's used as an authentication layer for 0Auth.

## Authorization and Authentication flows

1. Authentication is the process of verifying who a user is, while authorization is the process of verifying what they have access to.
2. For regular web apps. Exchanges an authorization code for a token.
3. For mobile and native applications. Same as above but first they need to use a proof key before the code exchange.
4. For public clients, or apps that are unable to securely store client secrets. It offers a streamlined workflow if the app only needs an ID token to perform user authentication.
5. For M2M applications, the system authenticates and authorizes the app rather than a user
6. The device asks the user to go to a link on their computer or smartphone to authorize the device. This is commonly used on devices that are difficult for users to enter text
7. Not recommended, should only be used when redirect-based flows cannot be used. Highly-trusted applications can request that users provide credentials, typically using an interactive form.
