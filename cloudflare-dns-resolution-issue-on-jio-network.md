---
description: We are not able to resolve IP address on Coudflare proxied mode on Jio.
---

# Cloudflare DNS Resolution Issue on Jio Network



**Jio Mobile Data; REFUSED Err; No IP resolved**

Jio Mobile Data DSN Server: fe80::b08c:75ff:fe94:2464%14#53(fe80::b08c:75ff:fe94:2464%14)

Blocks: a64f0cfbd3b3be47bcbddf2bc442ffde.r2.cloudflarestorage.com

<figure><img src=".gitbook/assets/Jio Mobile Data.jpg" alt=""><figcaption></figcaption></figure>





**JioFiber; No issues**

JioFber DNS Server: 2405:201:f024:3840::c0a8:1d01#53(2405:201:f024:3840::c0a8:1d01)

Doesn't block a64f0cfbd3b3be47bcbddf2bc442ffde.r2.cloudflarestorage.com

<figure><img src=".gitbook/assets/Jio Fiber.jpg" alt=""><figcaption></figcaption></figure>







**Jio Mobile Data w/ Custom DNS resolver; no issues**

<figure><img src=".gitbook/assets/Jio Mobile Data with custom resolver.jpg" alt=""><figcaption></figcaption></figure>







**Other network; No issues**

<figure><img src=".gitbook/assets/Other network.jpg" alt=""><figcaption></figcaption></figure>





**How to reproduce in Android Phone with JIO Data:**\
Install App like Termux:\
[https://play.google.com/store/apps/details?id=com.termux\&hl=en\_IN](https://play.google.com/store/apps/details?id=com.termux\&hl=en_IN)\
\
IPV6 DNS resolver wont resolve.

`curl -6 -v "https://tenant00140-apac-leeb-36efab44-pub-sb.hamanahel.app/config/index.json"`

IPV4 DNS resolver will resolve.\
`curl -4 -v"https://tenant00140-apac-leeb-36efab44-pub-sb.hamanahel.app/config/index.json"`
