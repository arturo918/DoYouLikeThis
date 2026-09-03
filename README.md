# WhoLikedThat

A Kahoot-style trivia game where players guess who interacted with specific TikTok videos within a group.

The app generates real-time questions based on actual user likes, favorites, and shares retrieved through official APIs.

## How it works

1. Players create or join a lobby and authenticate via TikTok.
2. The app fetches authorized interaction data.
3. Players compete to identify which group member liked, saved, or shared each displayed video.

## Backend Architecture

* Auth: OAuth 2.0 flow powered by TikTok Login Kit.
* Data Fetching: Async queries to the TikTok Data Portability API upon room entry.
* Caching: Up to 200 interaction records per user stored in SQLite to optimize API usage during active games.
* State Management: Express server handles room instances and matches overlapping player data for round generation.

## Tech Stack

* Frontend: React, Vite, TypeScript, Tailwind CSS
* Backend: Node.js, Express, TypeScript
* Database: SQLite
* APIs: TikTok Login Kit, TikTok Data Portability API

## Local Development

1. Clone the repository and install dependencies:

```git clone https://github.com/arturo918/WhoLikedThat-.git``
cd WhoLikedThat-
npm install```

2. Create a .env file in the project root:

```TIKTOK_CLIENT_KEY=your_client_key_here``
TIKTOK_CLIENT_SECRET=your_client_secret_here
REDIRECT_URI=https://arturo918.github.io/WhoLikedThat-/
PORT=3000```

3. Start the dev server:

```npm run dev```

## Legal & Compliance

* [Privacy Policy](https://arturo918.github.io/WhoLikedThat-/privacy.html)
* [Terms of Service](https://arturo918.github.io/WhoLikedThat-/terms.html)
* [Support](https://arturo918.github.io/WhoLikedThat-/support.html)
