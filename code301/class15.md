# Reading Notes

## What is OAuth

What is OAuth?

OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

Give an example of what using OAuth would look like.

Using OAuth can be illustrated with the example of a web application obtaining permission from users to access their Google Drive to store files. In this scenario, the application initiates the OAuth 2.0 flow by redirecting the user to Google's authorization server, where the user authenticates and grants the requested permissions. Subsequently, the user is redirected back to the application with an access token, which the application can then use to access the user's Google Drive. This process allows the application to access specific data while keeping the user's credentials private

How does OAuth work? What are the steps that it takes to authenticate the user?

Let’s assume a user has already signed into one website or service (OAuth only works using HTTPS). The user then initiates a feature/transaction that needs to access another unrelated site or service. The following happens (greatly simplified):

1.The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.

2.The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.

3.The first site gives this token and secret to the initiating user’s client software.

4.The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).

5.If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.

6.The user approves (or their software silently approves) a particular transaction type at the first website.

7.The user is given an approved access token (notice it’s no longer a request token).

8.The user gives the approved access token to the first website.

9.The first website gives the access token to the second website as proof of authentication on behalf of the user.

10.The second website lets the first website access their site on behalf of the user.

11.The user sees a successfully completed transaction occurring.

12.OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

What is OpenID?

OpenID is designed to be simple and extensible, and it allows users to manage their identities across different websites with the convenience of a single set of credentials. It also promotes the idea of decentralized identity, where users have more control over their personal information.

### Resources

What is the difference between authorization and authentication?

Authentication focuses on verifying the user's identity, while authorization controls and limits the user's access to specific resources or actions.

What is Authorization Code Flow?

the Authorization Code Flow is a fundamental OAuth 2.0 grant type that provides a robust and secure way for applications to obtain access tokens from an authorization server.

What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

The Proof Key for Code Exchange (PKCE) is an extension of the standard OAuth 2.0 Authorization Code Flow. It is designed to enhance the security of the authorization process, particularly for public clients such as native or single-page applications, which are unable to securely store a client secret.

What is Implicit Flow with Form Post?

The Implicit Flow with Form Post is an authentication flow used in the context of single-page applications (SPAs) to obtain ID tokens.

What is Client Credentials Flow?

The Client Credentials Flow is an OAuth 2.0 grant type that allows an application to securely act on its own behalf, without the involvement of a user.

What is Device Authorization Flow?

The Device Authorization Flow, also known as the Device Flow, is an OAuth 2.0 extension designed to facilitate user authentication and authorization on devices with limited input capabilities, such as smart TVs, IoT devices, and printers.

What is Resource Owner Password Flow?

The Resource Owner Password Flow (ROPC) is an OAuth 2.0 grant type that allows highly-trusted applications to directly obtain an access token by requesting that users provide their credentials (username and password) typically using an interactive form.

[What is OAuth? How the open authorization framework works](https://www.csoonline.com/article/562635/what-is-oauth-how-the-open-authorization-framework-works.html)

[Chat GPT](https://chat.openai.com/)
