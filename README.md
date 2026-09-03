# WhoLikedThat

A multiplayer party game where you and your friends try to guess who interacted with what on TikTok. Think Kahoot, but the questions are generated from your actual TikTok likes, favorites, and shares.

## What it actually does

You create a lobby, everyone logs in with their TikTok account, and the app builds trivia rounds out of your combined activity history. During each round, a video pops up and you have to call out which friend liked it, favorited it, or sent it to the group.

## How it works under the hood

1. **Auth:** Players authenticate using TikTok Login Kit (standard OAuth 2.0 flow).
2. **Data Retrieval:** The backend queries the TikTok Data Portability API asynchronously to pull recent likes, favorites, and shares.
3. **Storage & Caching:** We cache up to 200 interaction records per user locally in SQLite to build the game rounds without spamming the API.
4. **Lobbies:** Rooms sync player states and render real-time questions based on overlapping user data.

## Tech Stack

* **Frontend:** React, Vite, TypeScript, Tailwind CSS
* **Backend:** Node.js, Express, TypeScript
* **Database:** SQLite
* **APIs:** TikTok Login Kit, TikTok Data Portability API

## Running locally

First, clone the repository and install dependencies:

```bash
git clone [https://github.com/arturo918/WhoLikedThat-.git](https://github.com/arturo918/WhoLikedThat-.git)
cd WhoLikedThat-
npm install
