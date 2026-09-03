# WhoLikedThat

hacked this together over the weekend so my friends and I could play a kahoot-style trivia game with our actual tiktok activity. 

turns out guessing who favorited what at 3am gets pretty funny.

## what is this?

basically a web game where everyone joins a lobby, logs in through tiktok, and the app throws together trivia rounds based on what you've liked, saved, or sent around. 

a video comes up on screen and you have to call out who interacted with it.

## backend stuff

* **Auth:** Standard OAuth2 using TikTok Login Kit.
* **Data Retrieval:** Backend hits the TikTok Data Portability API asynchronously when players drop into the lobby.
* **Caching:** Saves up to 200 interaction records per user locally using SQLite so we don't spam TikTok's rate limits mid-game.
* **State sync:** Express manages room states & matches overlapping user data to spin up the rounds.

## Tech Used

* **Frontend:** React, Vite, TypeScript, Tailwind CSS
* **Backend:** Node.js, Express, TS
* **Database:** SQLite
* **APIs:** TikTok Login Kit & Data Portability API

## Running it locally

Clone it & install deps:

```bash
git clone [https://github.com/arturo918/WhoLikedThat-.git](https://github.com/arturo918/WhoLikedThat-.git)
cd WhoLikedThat-
npm install
