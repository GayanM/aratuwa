#OAuth 2.0 Token Introspection API for WSO2 Identity Server

* 1. Checkout and build the code from https://github.com/facilelogin/aratuwa/tree/master/api-security/org.wso2.carbon.identity.oauth.introspection  and deploy it as a war file in IS 5.1.0 (IS_HOME/repository/deployment/server/webapps/). 
* 2. Restart the Identity Server and now you should be able to use the introspection API.
* 3. Find below the usage of the introspection API. 

 ```javascript
     Empty Token:
     curl -k -H 'Content-Type: application/x-www-form-urlencoded' -X POST --data 'token=' https://localhost:9443/introspect
     
     Response: {"active":false} 
     
```