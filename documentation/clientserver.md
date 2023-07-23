---
title: Client-server communication
---

OpenHellion uses Nakama as a main server. The tasks the main server handles are: user accounts, friends, achievements (todo), match handling, chat, character info (todo), parties (todo), and notifications (todo). Later I wish to expand the tasks of the main server to include saving the world and more.

The most important task of the main server is the facilitate the connections between the client and the game server. The game server handles the simulation of the world, which is the game you actually play. This is done by using a small relay layer on the main server. The server sends a message to the main server using RPC, which then sends a message through the Nakama match system.

![A diagram showing how the clients and servers interact with Nakama.](res/ClientServer.drawio.svg)


![An example of how connections between client and server is handled.](res/CommunicationExample.drawio.svg)
