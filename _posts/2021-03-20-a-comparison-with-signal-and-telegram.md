---
title: "A comparison with Signal and Telegram"
---

Ansyble is in many ways a theoretical endeavor. It has a stylistic personality, but I would not have made it if I only felt there were stylistic deficiencies in the existing menagerie of common messaging applications. In this post, we'll discuss how Ansyble differs from Signal and Telegram on the backend with a focus on data, cryptography, and distribution, and how this manifests in the user experience.

### Signal

At a high level, Signal ties security to your device, while Ansyble ties security to your password. (Ansyble currently does not support two-factor authentication. This would certainly change if it actually got a userbase.)

#### Cryptographic protocol

Signal's crypotographic protocol is really quite good. I'm not aware of many theoretical deficiencies, and I essentially used the Signal protocol with Ansyble.

I did notice one minor deficiency: After you send a message and Signal updates your encryption keys, the next time your keys will be updated is when you get a reply. In a one-sided chat, this could mean that keys are not updated for a long time. In contrast, Ansyble will update your keys on every single message in a conversation, as long as your friend is _logged in_.

#### Portability

Signal is not portable. This is by design. The main advantage is self-explanatory: Eve essentially cannot eavesdrop without your phone in hand.

On the other hand, there are a host of disadvantages:

1. _You_ cannot use Signal or access your messages except on your phone.
2. Messages can be easily lost, unless manually backed up.
3. Switching devices is a headache.
4. There is a fractured experience in general, with separate apps for each OS and platform.

In contrast, Ansyble is built using the relatively new Progressive Web App (PWA) framework. This means it is built entirely with HTML and Javascript, and runs on any device with a modern browser, with essentially the same user experience. It is designed to be portable: The app itself is available on public devices with no installation, and your account data is acessible from any device via a password. 

#### Device footprint vs. forward secrecy

Is Ansyble less secure than Signal? In some ways, yes. In particular, forward secrecy is compromised. This means that there is a single piece of data (your password) which compromises your entire message history.

On the other hand, due to its minimal device footprint, Ansyble enjoys forms of security that Signal cannot. Since it is designed for nearly complete functionality on public devices, you do not lose much functionality by treating your own device as a public device. Precisely: If you do not store your Ansyble password on your phone, Eve cannot read your Ansyble messages even with your phone in hand.

In contrast, with Signal, if someone physically obtains your device, your entire message history is compromised. It's also worth bringing up Telegram's criticism of Signal's security model: The typical user does want to back up their messages, and if they do, they're likely to use something like Google drive, which is unencrypted, entirely defeating the purpose of end-to-end encryption.

#### Telegram

Telegram is essentially not encrypted. Rather, it supports end-to-end encrypted "secret chats" as a temporary communication channel, like a video chat. It's kind of a strange feature to have, because if I truly had something extraordinarily sensitive that I deliberately wanted Telegram not to access, I would use Signal or real life (or Ansyble!).

In contrast, Ansyble is _always_ end-to-end encrypted. In particular, all features are entirely compatible with its encryption.

I should add that Telegram is unlikely to change, because Telegram is at its heart, an unencrypted, public platform. The inescapable issue is that end-to-end encryption does not scale well, while the main draw of Telegram is its support for large communication channels. I've heard it does this very well. 

It's unfortunate that people put Telegram in the same sentence as Signal; Telegram fits much better in a category with Twitter, Facebook, Twitch, etc.

