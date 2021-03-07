+++
description = "Use RabbitControl with Java"
title = "Java"
draft = false
weight = -10
bref="RCP model and transporter"
+++



### Get the package for

maven:
```
<dependency>
  <groupId>cc.rabbitcontrol</groupId>
  <artifactId>rcp</artifactId>
  <version>0.3.26</version>
</dependency>
```

gradle:
```
implementation 'cc.rabbitcontrol:rcp:0.3.26'
```

rcp-java supports java >= 1.6

### Source
see: https://github.com/rabbitControl/rcp-java

### Example
``` java
RCPServer rabbitServer = new RCPServer();

final WebsocketServerTransporterNetty transporter = new WebsocketServerTransporterNetty();

rabbitServer.addTransporter(transporter);

transporter.bind(10000);

// expose parameter
Int32Parameter floatParameter = rabbitServer.createInt32Parameter("Int 32");

// update server (push to clients)
rabbitServer.update();
```
&nbsp;

---
Use a [app]({{< relref "/apps" >}}) to control exposed parameters.

&nbsp;
