# This repository has code for running a procedurally generated tower defense game.

A new player starts playing the game and a randomly generated domain is created.

A domain is a 2-d rectangular grid, attached at the perimeter to one or more other domains.

A player uses a game client (mobile app, say), to take game actions, including viewing visibile game state.

One or more game API servers provide clients with game state updates.

----------------------
Client-Server API:

  All operations are POSTs over HTTPS.

  /new
    Creates a new domain and returns it to the client.
