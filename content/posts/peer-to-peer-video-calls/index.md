+++
author = "Matt Lilley"
title = "Peer to peer video calling"
date = "2021-01-11"
description = "My mind was blown today when I found out about WebRTC and how it can enable video calls directly from my browser to yours without any data going through another server 🤯."
subtitle="It's built into your browser already 😮"
tags = [
    "technology"
]
+++

My mind was blown today when I found out about WebRTC and how it can enable video calls directly from my browser to yours without any data going through another server 🤯. I'm aware that I'm probably very late to the party on this one, but I was particularly excited by the [PeerJS](https://peerjs.com/) library that helped me get started really quickly. 

> PeerJS wraps the browser's WebRTC implementation to provide a complete, configurable, and easy-to-use peer-to-peer connection API. Equipped with nothing but an ID, a peer can create a P2P data or media stream connection to a remote peer.

I've had a lot of fun today building this little prototype and trying it out with friends:

{{< iframe src="https://glitch.com/embed/#!/embed/useful-tang?path=script.js&previewSize=100">}}

and because I've deployed the code as a Glitch app you can [remix it to your hearts content](https://glitch.com/edit/#!/useful-tang).
