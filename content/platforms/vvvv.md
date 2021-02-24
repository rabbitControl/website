+++
description = "Use RabbitControl with vvvv"
title = "vvvv"
draft = false
weight = -10
bref="Here is how to expose parameters from vvvv"
+++

[![VVVV-beta](/logos/vvvv.png#center)](https://vvvv.org/)

For updates see: https://discourse.vvvv.org/t/rabbitcontrol/16628

## vvvv gamma or VL

Required NuGet: [VL.IO.RCP](https://www.nuget.org/packages/VL.IO.RCP)  
Watch this video to learn [How to use NuGets](https://youtu.be/-U_kUQ3VDog)

## vvvv beta

Available since beta 39: Simply create a node called Rabbit (RCP) and configure its Host and Port inputs if necessary. Now you can already connect to this server using an [app]({{< relref "/apps" >}}).

Next you can start exposing parameters by creating IOBoxes, selecting them and pressing Ctrl+K. Any exposed IOBox will show up in all connected clients and can now be controlled bidirectionally, ie. either via any of the clients or in the patch.

To set some specific options (like min, max for values), select the IOBox in the Inspektor (Ctrl+I) and configure the options. Note that some of the options still won't autoupdate and you'll have to un- and re-expose the IOBox for them to take effect.

---
Use a [app]({{< relref "/apps" >}}) to control exposed parameters.
