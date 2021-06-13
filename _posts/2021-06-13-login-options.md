---
title: "Ansyble's many login options"
---

Here is an explanation of the login options for Ansyble.

### Save nothing personal (default)

By default, Ansyble's persistent storage contains no personal data, except your username. This means that your display name (first and last), password, encryption key, messages, etc. all vanish immediately if for instance, you pull the battery from your device.

The most annoying property of this login option is perhaps that push notifications cannot be read in plaintext: Since your encryption key is not stored, the message cannot be decrypted. You will only receive notifications that indicate the presence of a new message.

### Save encryption key only

This is a nice option because you don't need to log in every time you load Ansyble. Further, push notifications can now be read in plaintext. 

### Save encryption key and message data (not yet implemented)

This is the most similar to the login options for other common messaging apps. You can read messages offline, provided that they have been loaded previously while connected to the internet.

### Save everything, exclusively (Signal protocol)

This is essentially an implementation of the Signal protocol. The main advantages here are: 

1. Messages load quickly, similar to the previous option.
2. Messages enjoy [perfect forward secrecy](https://en.wikipedia.org/wiki/Forward_secrecy).

The main disadvantages are:

1. This obviously leaves all of your messages accessible on your device.
2. Your messages will not be accessible from other devices.

__Note:__ Existing chats that were initiated online will continue to be stored and accessible via the cloud. Only __new__ chats (initiated either by you or your contacts) will enjoy perfect forward secrecy.

### Simulate how the server sees your data

This simulates what developers and attackers can reconstruct from the data that is stored on Ansyble's servers, ie. without your password.

You will find that the server can see a surprisingly large amount of information about you. However, I claim that no other centralized messaging app can prove to you that they collect anything less. For instance, Signal claims that they collect almost no information about you, but it is impossible for them to prove this. Everything that Ansyble collects, Signal might be secretly collecting as well.

In other words, Ansyble's privacy claims are both trustless and optimal. If there is a protocol that can prove a piece of data is inaccessible to the server, Ansyble implements it. On the other hand, Ansyble essentially collects everything it cannot prove to you that it does not collect.

(This is slightly inaccurate: Ansyble does not collect login timestamps or IP addresses at the time of writing.)
