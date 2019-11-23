+++
description = "Use RabbitControl with the webclient"
title = "webclient"
draft = false
weight = -10
bref="Here is how to use the webclient"
+++

## Launch Client  
- From any browser (desktop or mobile) open this URL:
https://rabbitcontrol.github.io/client

- Enter Host and Port of your RabbitControl server application and click Connect.

<div style="margin-left: 30px;">
NOTE: Connecting to an unsecure websocket from secure context.  
You may need to adjust your browser settings!  
<u>Firefox:</u>  
Please set in 'about:config': 'network.websocket.allowInsecureFromHTTPS' to 'true'.
</div>
<br>

After connecting to a rabbitControl server you should now see all exposed parameters. e.g.:

{{< figure src="webclient.png" >}}
