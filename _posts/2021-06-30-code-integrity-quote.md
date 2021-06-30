---
title: "Code integrity"
---

Because Ansyble is a web app, its code can be updated by the server at will. This means that even if you verify that Ansyble's code uses secure encryption protocols, it might be tampered with as soon as you "look away."

To address this, upon installation, all authentic versions of Ansyble's code will save a random quote to your device as a cookie. This code is not shared with Ansyble's server, and is always on display while the web app is running. The code is instructed to delete this quote immediately if it is about to be replaced.

As a result, you can see when Ansyble's code has been updated (and Ansyble's server cannot reliably conceal this fact, since it doese not know which quote is on your device). Precisely, if you notice that Ansyble is running with a new or missing quote,

1. Ansyble was recently updated.
2. You're running on incognito mode, which disallows cookies.
3. You're not using your usual device.
4. Someone has infiltrated your connection to Ansyble and is sending you code which may have been tampered with.
