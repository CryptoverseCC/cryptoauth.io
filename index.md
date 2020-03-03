# Welcome to Cryptoverse Auth

In short it's Ethereum Wallet to *OpenID Connect* bridge.

This means that any software that implements *OpenID Connect* authentication mechanism is able to use **Cryptoverse Auth** as so called *Identity Provider* and login users that have Ethereum Wallet without requiring anyone to create any accounts or register anywhere.

You problably know those buttons "Login with Facebook" or "Signin with Google". It's the same thing. In both cases the process of validating the the user is really the user he/she is claiming to be is outsourced to external party (Facebook or Google in those cases). With *Cryptoverse Auth* you are able to do the same, the difference is that it validates that you are the owner of certain Ethereum address and tells the site that yes you really hold private keys to this address and that the site should use this address as your identity instead of your personal info.

You might ask how the site owner will reach you if the only information they receive is your Ethereum address? 
ETHMail to the rescue. By default *Cryptoverse Auth* passes your dedicated email address to the site your are login into. Those emails have a form of 0xYourAddress@ethmail.cc. You can see **Cryptoverse Auth** and **ETHMail** working together at https://web.ethmail.cc/

## Contact

You can contact me at 0x3b4361d03567a941877299f49b938f050c468651@ethmail.cc
