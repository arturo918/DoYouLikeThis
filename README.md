# WhoLikedThat

I built this party game to figure out which of my friends actually liked or saved specific TikToks. Basically Kahoot, but using our real TikTok history.

## What's the idea?

You set up a room, everyone signs in with TikTok, and the app mixes everyone's public activity into trivia questions. A video shows up on screen and you gotta guess who liked it, favorited it, or sent it to the group chat.

## How the backend handles it

* **Auth flow:** Standard OAuth 2.0 via TikTok Login Kit. Nothing fancy here.
* **Data fetching:** Backend queries TikTok's Data Portability API asynchronously when a player joins.
* **Caching:** Stores up to 200 activity records per user in SQLite so we don't hit API rate limits mid-game.
* **State sync:** Express handles room states and matches overlapping player interactions to build the rounds.

## Tech Stack

* **Frontend:** React + Vite, TypeScript, Tailwind
* **Backend:** Node.js, Express, TypeScript
* **Database:** SQLite
* **APIs:** TikTok Login Kit & Data Portability API

## Local Setup

Grab the repo and install packages:

```bash
git clone [https://github.com/arturo918/WhoLikedThat-.git](https://github.com/arturo918/WhoLikedThat-.git)
cd WhoLikedThat-
npm install
