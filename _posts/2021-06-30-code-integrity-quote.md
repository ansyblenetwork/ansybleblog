---
title: "Code integrity"
---

Because Ansyble is a web app, its code can be updated by the server at will. This means that even if you verify that the code your browser receives currently uses secure encryption, it might be replaced on your next visit.

To address this, upon installation, all authentic versions of Ansyble's code will save a random quote to your device as a cookie. This quote is not shared with Ansyble's server, and is always on display while the web app is running. The code is instructed to delete this quote immediately if new or updated code is about to be installed.


As a result, you can see when Ansyble's code has been updated (and the new code cannot reliably conceal this fact, since it does not know which quote was on your device). Precisely, if you notice that Ansyble is running with a new or missing quote, one of the following has occurred:

1. Ansyble was recently updated.
2. You're running on incognito mode, which disallows cookies.
3. You're not using your usual device.
4. Someone has infiltrated your connection to Ansyble and is sending you code which may have been tampered with.
