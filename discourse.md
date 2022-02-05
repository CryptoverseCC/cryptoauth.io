# Integrate Discourse with Cryptoverse Login (a.k.a. Cryptoauth)

## Get Client ID and Client Secret

To be able to use ethereum wallet login with your discourse instance you need client ID and client Secret.
You can obtain them by calling registration API:

```
> curl --header "Content-Type: application/json" \
    --request POST \
    --data '{"redirect_uris":["https://client.example.org/callback"],"token_endpoint_auth_method": "client_secret_basic"}' \
    https://login.cryptoverse.cc/oauth2/register -v
...
```

Remember to pass proper **redirect_uris**

## Install OpenID Connect Plugin

Install plugin [CryptoverseCC/discourse-openid-connect](https://github.com/CryptoverseCC/discourse-openid-connect) at your discourse instance, you can also use official one [discourse/discourse-openid-connect](https://github.com/discourse/discourse-openid-connect) but it's missing some features like ENS support.

## Configure your Discourse
Not all are necessary for login to work.

Discovery document url: [https://login.cryptoverse.cc/.well-known/openid-configuration](https://login.cryptoverse.cc/.well-known/openid-configuration)

![---](discourse-openid.png "Discourse - OpenID plugin settings")
![---](discourse-login.png "Discourse - Login settings")
![---](discourse-users.png "Discourse - Users settings")

<script type="text/javascript">window.$crisp=[];window.CRISP_WEBSITE_ID="82c167b2-b01f-43a2-80f1-4e18badcbc52";(function(){d=document;s=d.createElement("script");s.src="https://client.crisp.chat/l.js";s.async=1;d.getElementsByTagName("head")[0].appendChild(s);})();</script>
