# 🧭 Compass — Pirate Social

A pirate-themed social media platform built for the Solana ecosystem. Users can post, comment, follow trending content, and hover over token contract addresses (CA) to see live market data right in the feed.

## ✨ Features

- **Auth system** — email/password sign up and sign in
- **Feed** — create posts, comment, attach images
- **Trending** — surfaces the most popular posts
- **Radar** — *(token/project discovery section)*
- **Search & Notifications**
- **User profiles** and a settings page
- **CA Tooltip** — hovering over a contract address shows:
  - Live price, liquidity, and volume (via DexScreener API)
  - Risk score (based on liquidity/age)
  - 🐋 Whale & 🚀 Pump analysis badges
- **💎 Gem Hunt** — a mobile-friendly analysis panel that opens when tapping a CA
- **Page history / Back button** — SPA-style page navigation

## 🛠️ Tech Stack

- Vanilla HTML / CSS / JavaScript (single file, no framework)
- **Firebase Realtime Database** — stores users, posts, and comments
- **DexScreener API** — token market data (public endpoint)

## 🚀 Running it

It's a single HTML file, so there's nothing to install:

1. Clone or download the repo
2. Open `compass_mvp_release_v28_fix_async_tdz_comments_mobilefix_v12.html` in a browser

> Note: some browser security policies can behave oddly when opening the file directly by double-clicking. Running it through a simple local server (e.g. the VS Code "Live Server" extension) tends to be more reliable.

## ⚠️ Security Note

The Firebase configuration values (`apiKey`, `databaseURL`, etc.) are visible client-side — this is normal for Firebase and not a secret to protect. Actual security is enforced through **Firebase Console → Realtime Database → Rules**. Anyone using this project should review and configure their own Rules to prevent unrestricted read/write access.

## 📌 Status

Active development (MVP). Feedback and contributions welcome.
