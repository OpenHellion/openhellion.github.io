---
title: Client architecture
---

[The client](https://github.com/OpenHellion/Server) is the part of the project that the players interact with. It contains all of the graphical assets, handles rendering, and serves as an interface to the player.

![A diagram of the OpenHellion client architecture.](res/ClientArchitecture.drawio.svg){: height="400" .align-right}
As the diagram below shows, intialisation is handled by the InitializingScene, which when has completed, sends the player over to the Main Menu Scnene. This scene then sends the player to the Client scene. This scene has the responsibility for running the game.

In addition to this, there also exists many scenes for the various structures and celestial objects in the game. These are loaded and cached on initialisation and fetched when they are to be used in the game.
