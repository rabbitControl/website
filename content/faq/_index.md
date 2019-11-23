+++
draft= false
title = "FAQ"
description = "Asked and answered"
+++

## Can I use the protocol for a multi server/client scenario?
The protocol itself does not specify any special functions for a scenario like this. It should still be possible to use it for such scenarios though by providing specialized server/client implementations that deal with message dispatching. While out of scope for the initial implementation this could be re-considered for a later version.

## How do data providers and data clients find each other?
This will be by manual configuration in a first version as we consider automatic discovery out of scope of the protocol. In a later version we might consider adding DNS-SD (aka Zeroconf) or similar to the client/server implementations.

## Is there any transport defined in the protocol?
No, the protocol is transport agnostic. For streaming protocols (e.g.: TCP) you need to handle your own message framing. Our initial implementation will be for Websockets.

## How can I control parameters via hardware devices?
The protocol is primarily intended to allow for control of parameters via visual interfaces that are created ad-hoc/on-demand. The client UI is being created on the fly depending on the parameters exposed on a server. Combining this with 'static' hardware devices is of course possible but out of scope of the protocol. One would need to write a specialized client that can route individual hardware knobs/sliders to the exposed parameters.

## Is the protocol always sending every field in a Parameter?
No, the protocol is designed to only send the actual data you want to update.

## Does it support bangs?
Yes and if you're afraid of loosing bangs over an insecure transport (e.g. UDP) then choose a secure transport (e.g. TCP)

## Does it support arrays?
Yes, and even lists!

## Does it suppport datatype X?
Most likely and if not you can always build your own compound datatype.
