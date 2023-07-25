---
title: OpenHellion project documentation
---

![Image of the Hellion Project open in the Unity game engine.](https://user-images.githubusercontent.com/37084190/196989422-4079d0fe-c16a-416b-80f7-27df3077c366.png)

The OpenHellion project documentation aims to explain how the project is put together. This site is for more techical users wanting to get a more general understanding of how the game works.

## In overview
![A diagram of the OpenHellion server-client architecture.](res/ClientArchitecture.drawio.svg){: height="400" .align-right}
The project contains three major parts: the client, the server, and the main server. These three communicate with each other through several layers, a relay, Nakama's internal communcation, and using REST RPCs, as explained in the [Client-server communication](clientserver) article.

While the main server and server parts are tasked with more "under the hood" problems, the client is what the players see and use, and is therefore the most important part. This is explained more thoruoughly in the [Client architecture](client) article.
