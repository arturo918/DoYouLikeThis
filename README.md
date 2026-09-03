# WhoLikedThat

A Kahoot-style party game based on your group's TikTok activity. 

Players connect their TikTok accounts, and the app generates trivia rounds where everyone has to guess who among their friends liked, favorited, or shared a specific video.

## How it works

1. Log in with your TikTok account via official OAuth.
2. The app uses the TikTok Data Portability API to fetch interaction history.
3. Join a lobby with friends and test how well you know each other's TikTok feeds.

## Tech Stack

* **Frontend:** React, Vite, TypeScript, Tailwind CSS
* **Backend:** Node.js, Express, TypeScript
* **Database:** SQLite
* **APIs:** TikTok Login Kit & Data Portability API

## Development

```bash
# Clone the repo
git clone [https://github.com/arturo918/WhoLikedThat-.git](https://github.com/arturo918/WhoLikedThat-.git)
cd WhoLikedThat-

# Install dependencies
npm install

# Start local server
npm run dev
