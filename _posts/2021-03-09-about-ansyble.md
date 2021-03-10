---
title: "About Ansyble"
---

Ansyble is an app for online conversations. Unlike most other chat apps, it is built on the open web. This means that it can produce a comparatively seamless experience. For instance:

1. It's easy to get started: Just choose a username. There is no need for, or association with, phone numbers or emails.
2. Ansyble runs on any major browser (Chome, Firefox, or Safari), with no installation or downloads, on either mobile or desktop. Installing the native app is entirely optional/cosmetic.
3. Messages are synchronized in real-time between however many devices you happen to be using.
4. Messages are saved on the cloud, so you can immediately access and search them from any of those devices.
5. By default, Ansyble saves no personal information to your device.
6. All communications and personal data are end-to-end encrypted. Nothing appears as plaintext to Ansyble except usernames and timestamps.
7. You can easily export messages to CSV/Excel.
8. The interface is simple and optimized: Minimal so as to host the maximal number of features. (Modulo gifs and emojis; for those you are on your own.)
9. Everything is open source, in one small HTML file you can access from your browser's development tools.

In short, there should be a simple, fast, and fully functional username-based messaging application build on the modern browser. I wasn't aware of one, so I made one.

#### Who are you?

I'm a random stranger on the internet who might know a bit about coding and cryptography. You can contact me at: ansyblenetwork@gmail.com

#### Why can't I find Ansyble on Google?

I made Ansyble for fun during 2020. I'm not making any real effort on SEO or promotion. Ansyble may or may not grow; if it does, it will have been organically.

#### Does Ansyble make any money?

No.

#### Is my data safe on Ansyble? Will it be here tomorrow, next week, next month, etc?

This is a legitimate concern. So far, Ansyble has been up and running since March 2020, or at least one year. At the time of writing, Ansyble is free and effortless for me to run, so I have no reason to end the project.

I will make every effort to inform all users if support ends. (Until then, keep in mind that there is a convenient export-to-CSV/Excel function for your backup needs.)

#### Is my data safe FROM Ansyble?

Yes. All messages and personal data are end-to-end encrypted, and thus opaque to me and Ansyble. This is not just a default setting; there is no other setting.

#### How is Ansyble encrypted?

The protocol is essentially the Signal Protocol. However, unlike Signal, keys are stored on the cloud. These keys are encrypted using (a hash of) your password, so the end-to-end encryption is authentic. (However, this approach renders forward secrecy mostly meaningless. if you're paranoid, a true Signal Protocol option is available at login as well. In exchange, this option renders Ansyble's portability mostly meaningless.)

The cryptographic primitives are pulled from the state-of-the-art [Web Crypto API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Crypto_API).

#### Has a third party verified the encryption?

No. Ansyble is a one-person project and at the time of writing, essentially no one knows about it. 

However, the source code is always available to you (or any user) via your browser's development tools. If you're interested in the project and/or the encryption, I would be happy to discuss via email.

Note: I am aware of and waiting for action regarding [this](https://github.com/w3c/ServiceWorker/issues/822) theoretical concern.

#### Wait...is the icon inspired by that famous photograph, (xyz)?

YES. Contact me!!
