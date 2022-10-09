# Class 301 Reading15

## What is OAuth

1. What is OAuth?
    - OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

2. Give an example of what using OAuth would look like.
    - It is like when we first created our Github account and gitHub asked if we would like to login with google account.

3. How does OAuth work? What are the steps that it takes to authenticate the user?
    - The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
    - The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
    - The first site gives this token and secret to the initiating user’s client software.
    - The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
    - If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
    - The user approves (or their software silently approves) a particular transaction type at the first website.
    - The user is given an approved access token (notice it’s no longer a request token).
    - The user gives the approved access token to the first website.
    - The first website gives the access token to the second website as proof of authentication on behalf of the user.
    - The second website lets the first website access their site on behalf of the user.
    - The user sees a successfully completed transaction occurring.
    - OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

4. What is OpenID?
    - OpenID is for authintication and serves as a single sign-in, vouching for the identities of users.

## Authorization and Authentication flows

1. What is the difference between authorization and authentication?
    - Authentication verifies the identity of a user or service, and authorization determines their access rights.

2. What is Authorization Code Flow?
    - It exchanges an Authorization Code for a token. Your app must be server-side because during this exchange, you must also pass along your application's Client Secret, which must always be kept secure, and you will have to store it in your client.

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
    - During authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security. Additionally, single-page apps have special challenges. To mitigate these, OAuth 2.0 provides a version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange (PKCE).

4. What is Implicit Flow with Form Post?
    - As an alternative to the Authorization Code Flow, OAuth 2.0 provides the Implicit Flow. It is for Public Clients, or applications which are unable to securely store Client Secrets.

5. What is Client Credentials Flow?
    - Machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user.

6. What is Device Authorization Flow?
    - With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device.

7. What is Resource Owner Password Flow?
    - A highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form.

## Things I Want To Know More About

- More react, react, react!!!!

## Sources

- https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html

- https://auth0.com/docs/get-started/authentication-and-authorization-flow
