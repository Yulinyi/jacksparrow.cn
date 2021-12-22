---
title: '常用的物联网ioT协议'
published: false
---
 在物联网协议中，我们一般分为两大类：
 - [x] 一类是传输协议
 - [x] 一类是通信协议。

![](https://gitee.com/helloyuzz/sharepic/raw/master/iot.png)
传输协议一般负责子网内设备间的组网及通信；
通信协议则主要是运行在传统互联网TCP/IP协议之上的设备通讯协议，负责设备通过互联网进行数据交换及通信。

#### 1.REST/HTTP，松耦合服务调用
 - 无状态CRUD的 HTTP 方法，比如：GET、PUT、POST 和 DELETE。

#### 2.CoAP协议
 - CoAP (Constrained Application Protocol)，受限应用协议，应用于无线传感网中协议，支持缓存：CoAP协议支持资源描述的缓存以优化其性能。

#### 3. MQTT协议(低带宽)
 - MQTT (Message Queuing Telemetry Transport )，消息队列遥测传输，由IBM开发的即时通讯协议，相比来说比较适合低带宽、不可靠的物联网场景。
  
#### 4. DDS协议(高可靠性、实时)
 - DDS(Data Distribution Service for Real-Time Systems)，面向高可靠性、实时传输系统的数据分布服务。
 
#### 5. AMQP协议(互操作性)
 - AMQP(Advanced Message Queuing Protocol)，先进的面向消息、队列消息（发布/订阅）协议，用于业务系统例如PLM，ERP，MES等进行数据交换。

#### 6. XMPP协议(即时通信)
 - XMPP(Extensible Messaging and Presence Protocol)可扩展基于XML通讯的分布式网络和表示协议，一个开源形式组织产生的网络即时通信协议。

#### 7. JMS (Java Message Service)
 - JMS (Java Message Service)，即消息服务，这是JAVA平台中著名的消息队列协议。