# 🎙️ GitHub Sound

> **The world codes. We narrate.**

A silly, lighthearted web app that streams GitHub's public events and **reads them aloud** using your browser's text-to-speech — with karaoke-style word highlighting as each word is spoken.

## ✨ Features

- 🔴 **Live stream** — polls `api.github.com/events` respecting `X-Poll-Interval`
- 🎤 **Text-to-speech** — commit messages, PR titles, issue descriptions spoken aloud
- 🎵 **Karaoke display** — each word lights up as it is spoken
- 🃏 **Event cards** — colourful, bouncy cards for pushes, issues, PRs, releases & more
- 🤫 **Bot filtering** — silences dependabot, renovate & friends
- 🔑 **Optional GitHub token** — paste a PAT to raise the rate limit from 60 → 5000 req/hr (saved to `localStorage`)
- ⏸ **Pause / mute** — take a breather whenever you need
- 🌐 **GitHub Pages ready** — pure static HTML, zero build step

## 🚀 Usage

Visit the [GitHub Pages site](../../) or open `index.html` in any modern browser (Chrome recommended for best speech boundary support).

To get a GitHub token: **Settings → Developer settings → Personal access tokens → Fine-grained** — no scopes required for public events.

## 🗂 Event types

| Badge | What happened |
|-------|---------------|
| `push` | Commit messages (merge commits skipped) |
| `PR` | Pull request opened / merged |
| `issue` | Issue opened |
| `comment` | Issue & review comments |
| `create` | New repository created (with description) |
| `release` | Package / version released |
