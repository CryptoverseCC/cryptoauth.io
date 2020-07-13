# Welcome to Cryptoverse Login

In short it is an Ethereum Wallet to *OpenID Connect* bridge.

This means that any software that implements the *OpenID Connect* authentication mechanism is able to use the **Cryptoverse Login** as so called *Identity Provider* and login users that have Ethereum Wallet without requiring anyone to create any accounts or register anywhere.

You problably know those buttons "Login with Facebook" or "Signin with Google". It's the same thing. In both cases the process of validating the the user is really the user he/she is claiming to be is outsourced to external party (Facebook or Google in those cases). With *Cryptoverse Auth* you are able to do the same, the difference is that it validates that you are the owner of certain Ethereum address and tells the site that yes you really hold private keys to this address and that the site should use this address as your identity instead of your personal info.

You might ask how the site owner will reach you if the only information they receive is your Ethereum address? 
ETHMail to the rescue. By default *Cryptoverse Auth* passes your dedicated email address to the site your are login into. Those emails have a form of 0xYourAddress@ethmail.cc. 

## Showcase

You can see **Cryptoverse Login** in action at [https://ethmail.cc](https://ethmail.cc) and [https://community.cryptoverse.cc](https://community.cryptoverse.cc)

## Contact

You can contact me at [xunkulapchvatal@ethmail.cc](mailto:xunkulapchvatal@ethmail.cc)

<script type="text/javascript">window.$crisp=[];window.CRISP_WEBSITE_ID="82c167b2-b01f-43a2-80f1-4e18badcbc52";(function(){d=document;s=d.createElement("script");s.src="https://client.crisp.chat/l.js";s.async=1;d.getElementsByTagName("head")[0].appendChild(s);})();</script>
