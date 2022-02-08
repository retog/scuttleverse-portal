# scuttleverse-portal

What is a Scuttleverse Portal?

## Abstract

A Scuttleverse portal is a website where all user generated content is created by a Scuttlebutt client running in the browser. The user expirience is very similar to a regular website, but the user account is not tied to the website but a Scuttlebutt identity stored in the browser.

## Actors

The following actors and entities are essential for a Scuttleverse Portal.

### The User

The user is the person that uses the portal. The user is identified by a Scutlebutt FeedId and has access to the matching private key which is stored on the machine of the user (typically in the Browser's LocalStorage) and never sent over the network.

### The Portal Owner

The person that operates the portal and has access to its private key.

### The Portal Server

[1] The software running the web portal
[2] An instance of a portal server [1]
[3] A host or cluster running a portal server [2]

## Requirements

Any well behaving portal must satisfy these requirements.

### Key export

The user can export the Scuttlebutt secret and use it in another client.

### Websocket Connection to Portal

The browser client establishes a Scuttlebutt connection over a websocket connection to the origin host.

### Addtional Connections

The client can estabish a Scuttlebutt connection to any host their browser can establish a websocket connection.
