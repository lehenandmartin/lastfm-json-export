<h1 align="center">Last.fm JSON export</h1>
<h3 align="center">Download your full Last.fm scrobble history as a JSON file, right from your browser.</h3>

<p align="center">
  <img src="https://img.shields.io/github/license/lehenandmartin/lastfm-json-export" alt="License">
  <img src="https://img.shields.io/badge/HTML%20%2B%20JS-no%20dependencies-F7DF1E?logo=javascript&logoColor=black" alt="HTML + JS, no dependencies">
  <img src="https://img.shields.io/badge/Koito-proof-2ea44f" alt="Koito-proof">
</p>

<p align="center">
  <a href="https://lehenandmartin.github.io/lastfm-json-export/"><strong>Open Last.fm JSON export</strong></a> — runs in your browser, nothing to install
</p>

---

**The easiest way to use it is the hosted version: [lehenandmartin.github.io/lastfm-json-export](https://lehenandmartin.github.io/lastfm-json-export/).** Enter your Last.fm username and an API key ([get one here](https://www.last.fm/api/account/create)), click *Start export*, and the JSON file downloads when it's done.

Everything happens in your browser: the page talks directly to the Last.fm API, and your API key is never stored or sent anywhere else.

## Koito-proof

The file is an array of the raw pages returned by Last.fm's `user.getRecentTracks`, which is exactly what [Koito](https://github.com/gabehf/koito) reads. To import it, put the JSON file in Koito's `import/` folder and restart Koito.

## Features

- Full history, or a date range
- Page limit for a quick test (200 scrobbles per page)
- Pause and resume, even after closing the tab (progress is kept in your browser)
- Automatic retries when Last.fm or the network hiccups, at most 4 requests per second
- Clear messages for an invalid key, an unknown user or a private profile

## About

This project was built with the assistance of [Claude](https://claude.ai), under the author's direction and review.

## License

[MIT](LICENSE) — © 2026 Martin Le Hénand
