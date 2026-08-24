# IdeaQuantum Outliner — version feed

One file, `latest.json`, holding the newest released version of
[IdeaQuantum Outliner](https://github.com/Imaginativeone/my-electron-react-app).

The app fetches it on launch, compares against its own version, and shows a
banner if there is a newer one. It sends nothing: no version, no identifier, no
query string. It reads a static file and does the comparison locally.

This repository is public so that the app can read it without a token, while
the app's own source stays private. There is no code here and nothing else will
be added.

Written by `npm run announce` in the app's repo, which is part of the release
flow — a feed updated by hand is a feed that goes stale silently, and a stale
feed means the banner never appears and nobody finds out.
