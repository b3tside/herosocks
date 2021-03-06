# Heroku Shadowsocks Obfs TLS
Deploy shadowsocks server on heroku
## Principle
Simple-obfs convert the traffic into websocket instead of ordinary tcp connection, which could serve behind nginx. \
Theoretically, this enables ss-server to use any CDN that support websocket traffic, for example, Cloudflare.
## One-Click button
[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)
## How to use
Host: <app_name>.herokuapp.com \
Port: 443 \
Plug-in: simple-obfs or ss-local.exe \
Plug-in-options: obfs=http;obfs-host=<app_name>.herokuapp.com
## Note
This trick heavily relies on the domain of `herokuapp.com`. \
Please DO NOT distribute this repo everywhere in case the domain is blocked.
## Demo
Feel free to use but make sure you obey the Note part mentioned above. \
![](https://github.com/laintuv00/herosocks/blob/master/img/demo.png)
