# IdentityServer4.HybridFlow.NoConsent
IdentityServer4 sample using Hybrid flow and without a consent page.

### Addresses:

* [http://localhost:42705/](http://localhost:42705/) IdentityServer
* [http://localhost:34599/](http://localhost:34599/) Protected API
* [http://localhost:22507/](http://localhost:22507/) MVC Client

### Pages:

* [http://localhost:22507/web/protectedWeb](http://localhost:22507/web/protectedWeb)
  
  Page that requires login. 
  
  **Username:** test.user
  
  **Password:** password
* [http://localhost:22507/web/protectedAPI](http://localhost:22507/web/protectedAPI)
  
  Page which calls protected API.
* [http://localhost:42705/Login/Logout](http://localhost:42705/Login/Logout)
  
  Logout page. You need to close all browser windows and you may need to clear cookies.

### Remarks:

Console client uses Client Credential flow to make API call. Hence no "sub" claim in the token. MVC client login is on behalf of the user so the token does have "sub" claim.
