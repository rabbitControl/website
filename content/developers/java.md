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
  <groupId>io.github.rabbitcontrol</groupId>
  <artifactId>rcp</artifactId>
  <version>0.2.7</version>
</dependency>
```

gradle:
```
implementation 'io.github.rabbitcontrol:rcp:0.2.7'
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
Use a [client]({{< relref "/clients" >}}) to control exposed parameters.

&nbsp;
