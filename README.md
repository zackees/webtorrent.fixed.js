# webtorrent.fixed.js
An actively developed, compiled fork of Webtorrent with fixes carefully applied.

The following patches have been applied.

```
  const ICECOMPLETE_TIMEOUT = 1 * 1000

  Which SIGNIFICANTLY speeds up webtorrent.
  
  Made Tracker a global symbol.

  Made WebTorrent it's own symbol.

  Defensively blocked unchoking webSeeds:
    if (this.type === "webSeed") {
        console.log("webseed blocked unchocked, they are always choked.")
        return
    }
```
