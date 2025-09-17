---
layout: page
title: Web Socket Activity
nav_exclude: true
---

## Web Socket Activity
This project will give you practice in working with web sockets and the typed emitter pattern.

Start by downloading the [starter code]({{ site.baseurl }}{% link Examples/module-05-interaction-level-design.zip %}).

### Instructions
The current protocol, in `webSocketsSimple/shared.ts', has the server start the conversation with each client by sending it a `ping`

Modify this system in the following ways:
1. The server should keep track of the number of clients that are connected.
2. When a new client joins, the client should send the server a `hello` message with its name.
3. When the server sees the new client, it should print to the console the name of the new client and the total number of connected clients. It should then send an initial ping to the new client, as it does now.
4. When a client is disconnected, the server should print to the console the name of the client that is leaving and the updated number of connected clients.

Check your solution by running `npx ts-node demo-server.ts` in one shell window, and `npx ts-node demo-clientAB.ts` in a separate window.  Try starting the server first, and then the clients; then try starting the clients first and then the server. Observe the differences in behavior, if any. This check is for your purposes only, you need not submit it unless your instructor requires it in the Canvas assignment.

### Submission
Make your changes in the files in the `webSocketsSimple` directory. Add a README file to summarize what you did. Zip up that directory and submit it to the Canvas assignment for this activity.

### Grading
This activity is worth 10 points, 2.5 points for each of the four modifications listed above.  The graders will run your code to verify that it works as specified.