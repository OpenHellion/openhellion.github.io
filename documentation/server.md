---
title: Server architecture
---

[The server](https://github.com/OpenHellion/Server) is currently in the very early stages of a restructuring. The aim of this is to make the server run asynchronously, to both improve performance and reduce the total size of the codebase.

As explained in the [home page](home), the server is the part of the game that runs the actual simulation. The user will interact with the server through the client, by sending packets with Google protocol buffers.

![A diagram of the server architecture.](res/Server.drawio.svg)
