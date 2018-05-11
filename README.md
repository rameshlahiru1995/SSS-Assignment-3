# SSS-Assignment-3



######## Blog Post - https://technoholicsblog.blogspot.com/2018/05/secure-software-systems-assignment-3.html   ############ 


 SSS Assignment 03 - application that consumes the service of an OAuth…

… Authorization Server and an OAuth Resource Server.

● Send a request to the OAuth authorization server website for obtaining the access token. During the flow, it will prompt for user authentication (eg: facebook). You may use any supported OAuth grant type (eg: authorization code, implicit etc.).

● Once the OAuth access token is received, invoke the resource server APIs and obtain
the protected resources.

An example is implementing social login where you provide login with facebook/linkedin etc.
feature in your web application. However there is no restriction for your implementation. The
scope of this assignment is testing the use of OAuth framework. Therefore you may use your
creativity and implement your own idea to demonstrate OAuth flow. An example is, when the
user uses your web application, automatically updating user’s facebook status with some
message.


How to make this work

If you are not willing to change REDIRECT_URL

    Your localhost should be "https://localhost/../.."
   
    Copy https://localhost/Facebook-Social-OAUTH-2.0/index.php, https://localhost/Facebook-Social-OAUTH-2.0/server.php ,     
    
    https://localhost/Facebook-Social-OAUTH-2.0/redirect.php into your facebook APP "Valid OAuth Redirect URIs"
    
    Change follwing parameters in following functions.

    AUTH_URL($client_id,$redirect_url) -> change $client_id = your App id

    get_auth_code($client_id, $redirect_uri, $auth_code, $appID_secret_base64) -> change $client_id, 

    $appID_secret_base64=Base64(YourAppId:Secret)
    
    Done!
