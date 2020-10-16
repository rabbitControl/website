+++
description = "Use RabbitControl with the webclient"
title = "Webclient"
draft = false
weight = -10
bref="Here is how to use the webclient"
+++

## Launch Client  
From any browser (desktop or mobile) open this URL:  
http://client.rabbitcontrol.cc  
Enter Host and Port of your rcp server application and click Connect.

Or directly connect to an rcp server by providing ip:port in the URL like e.g:  
http://client.rabbitcontrol.cc/#192.168.0.23:10000

<div style="margin-left: 30px;">
NOTE: Connecting to an unsecure websocket from secure context.  
You may need to adjust your browser settings!  
<u>Firefox:</u>  
Please set in 'about:config': 'network.websocket.allowInsecureFromHTTPS' to 'true'.
</div>
<br>

After connecting to a rabbitControl server you should now see all exposed parameters. e.g.:

{{< figure src="webclient.png" >}}
