# webtorrent.fixed.js
An actively developed, compiled fork of Webtorrent with fixes carefully applied.

The following patches have been applied.

```
  const ICECOMPLETE_TIMEOUT = 1 * 1000
  Which SIGNIFICANTLY speeds up webtorrent.

  Replaced all instances of function process.nextTick with queueMicrotask to
  improve background performance. Tested to work well.
```
