---
date: 2025-04-01
title: When In Doubt Client Mode
author: Calvin Jutting ([@KN0CTJ](calvin@iowamesh.net))
---


## When In Doubt *Always* choose Client Mode (A guide to roles on our devices)

One of the things that need to be address up front as IowaMesh grows will be the appropriate use of the modes. Probably another controversial post much like the Ok to MQTT post, but it's a good chance for all of us to look at the choices we make and out it effects the Mesh

So Lets get on with it!
{{< imgproc "mr-t-fools.jpg" Resize "500x" >}}


Selecting the appropriate device role is crucial for maintaining an efficient and reliable Meshtastic mesh network. With recent updates to Meshtastic, certain roles have been refined or deprecated to enhance network performance. For mobile nodes and specific stationary scenarios, Client and Client Mute modes are often the most suitable choices. Let's explore these roles and discuss the implications of misapplying routing roles.​

Updated Meshtastic Device Roles:
Meshtastic nodes can be configured with various roles, each tailored to specific functions:
- Client: This is the default role for most nodes, enabling standard communication capabilities. Nodes in Client mode send and receive messages and participate in routing when necessary.

- Client Mute: Similar to Client mode but with routing disabled. These nodes send and receive their own messages without relaying messages for others, reducing network congestion in areas with high node density. ​

- Router: Intended for stationary nodes strategically placed to route messages and extend network coverage. Routers prioritize relaying messages from other devices and attempt to conserve power by reducing their own transmissions.

- Repeater: Functions similarly to a Router but focuses solely on rebroadcasting messages without originating its own. Repeaters are typically used to enhance coverage in specific areas. ​

- Router Late: A newer role designed for nodes that should act as routers but with a delayed rebroadcast, allowing other nodes to transmit first. This role helps in scenarios where a node is well-placed but should not dominate the routing process. ​

- Sensor: For devices primarily gathering and transmitting sensor data. While they can route messages, their main function is to report telemetry, even during high channel utilization. ​


***Notably, the Router-Client role has been deprecated in recent Meshtastic versions to simplify role assignments and improve network efficiency.​***

So lets look at some advantages and disadvantages

Advantages of Client and Client Mute Modes for Mobile Nodes:

- Network Efficiency
Mobile nodes in Client mode can participate in routing when necessary, but in areas with dense network coverage, this can lead to redundant transmissions. Switching to Client Mute mode in such scenarios prevents unnecessary rebroadcasts, reducing the risk of packet collisions and network congestion. ​
- Battery Conservation
Routing and rebroadcasting consume additional power. By operating in Client or Client Mute mode, mobile nodes conserve battery life, extending their operational duration—especially critical for handheld or portable devices.​
- Stability and Reliability
Mobile nodes frequently change positions, leading to variable connectivity. Assigning them as Routers can disrupt message paths when they move out of range. Keeping mobile nodes in Client or Client Mute mode maintains stable routing through strategically placed stationary routers.​

While stationary nodes often serve as Routers to extend network coverage, certain situations warrant using Client or Client Mute modes
Considerations for Stationary Nodes:
- Specific Use Cases: Nodes dedicated to particular functions, like sensors, may not need to route messages.​
- High-Density Areas: In environments with numerous nodes, excessive routers can lead to packet collisions and reduced network performance.

So what are the risks of misapplying Router and Repeater Roles:
- Increased Packet Collisions
- Overuse of Routers and Repeaters, especially in close proximity, can cause simultaneous rebroadcasts, leading to higher noise levels and packet errors. 
- Reduced Network Range
Improperly placed routers may consume message hops prematurely, preventing packets from reaching more strategically located nodes and limiting overall network range.​
-  Asymmetrical Links
- Poor router placement can result in one-way communication, where messages are sent but responses cannot return, disrupting effective two-way communication.​

Sometimes it’s hard not to be that guy but maybe with a little bit of explanation we can help make sure the mesh stays working well for everyone. 

{{< imgproc "Meshtastic-Router-Overdone.jpg" Resize "500x" >}}

So I might argue here that Client will be the choice of modes for most of us. I might even go as far as Client Mute especially if you are travling by plane. The traveler bridges larges area's for a while, but then breaks it again. Would love to hear your feedback as well! Hope this helps as we continue to grow the mesh here in Iowa!