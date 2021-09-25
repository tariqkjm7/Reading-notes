# Authentication



## OAuth definition:
**OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.**

`When trying to understand OAuth, it can be helpful to remember that OAuth scenarios almost always represent two unrelated sites or services trying to accomplish something on behalf of users or their software. All three have to work together involving multiple approvals for the completed transaction to get authorized.`

### How OAuth works
Let’s assume a user has already signed into one website or service (OAuth only works using HTTPS). The user then initiates a feature/transaction that needs to access another unrelated site or service. The following happens (greatly simplified):
* **The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.**
* **The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.**
* **The first site gives this token and secret to the initiating user’s client software.**
* **The client’s software presents the request token and secret to their authorization provider `(which may or may not be the second site)`**
* **If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website**
* **The user approves `(or their software silently approves)` a particular transaction type at the first website.**






### RECOMMENDED WHITEPAPERS
[Rely on Google Cloud for SAP, Today and Tomorrow](https://www.csoonline.com/resources/224672/rely-on-google-cloud-for-sap-today-and-tomorrow)

[Cognizant SAP on Google Cloud Video](https://www.csoonline.com/resources/224662/cognizant-sap-on-google-cloud-video)

[Doing business intelligently with a new ERP foundation](https://www.csoonline.com/resources/224709/ciso-guide-to-vendor-email-compromise-vec)
