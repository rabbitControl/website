+++
description = "Use RabbitControl with the webclient"
title = "webclient"
draft = false
weight = -10
bref="Here is how to use the webclient"
+++

## Launch Client  
From any browser (desktop or mobile) open this URL:
https://rabbitcontrol.github.io/client

Enter Host and Port of your RabbitControl server application and click Connect.

NOTE:
Connecting to an unsecure websocket from secure context. You may need to adjust your browser settings!

To allow this please set: 'network.websocket.allowInsecureFromHTTPS' in 'about:config' to 'true'.

You should now see any parameter exposed from your server application, like so:

{{< figure src="webclient.png" >}}
