# 🎮 WhoLikedThat - TikTok Trivia Game

**WhoLikedThat** is an interactive, Kahoot-style trivia web game where players guess which friend liked, favorited, or shared a specific TikTok video! 

By leveraging official TikTok APIs, players connect their accounts and turn their actual activity history into a fun, competitive multiplayer guessing game.

---

## 🌟 Key Features

* **TikTok Integration:** Authenticate securely via TikTok Login Kit and retrieve authorized interaction history through the Data Portability API.
* **Kahoot-Style Gameplay:** Real-time trivia rounds where players identify who among their group interacted with a displayed TikTok video.
* **Privacy & Security First:** Built strictly on top of official TikTok developer endpoints with no web scraping or unauthorized tracking.
* **Custom Game Lobbies:** Host private matches with friends and see who knows their group's TikTok habits best.

---

## 🛠️ Tech Stack

* **Frontend:** React, Vite, TypeScript, Tailwind CSS
* **Backend:** Node.js, Express, TypeScript
* **Database:** SQLite (limited local caching for recent activity)
* **APIs:** TikTok Login Kit, TikTok Data Portability API

---

## 🔒 Privacy & Compliance

This application strictly complies with TikTok Developer policies:
* **No credentials stored:** Authentication is handled end-to-end via official OAuth 2.0 flows.
* **Data Limits:** Data is fetched on-demand with strict retention policies and stored locally only as required for active game sessions.
* **Official Web Pages:**
  * [Privacy Policy](https://arturo918.github.io/WhoLikedThat-/privacy.html)
  * [Terms of Service](https://arturo918.github.io/WhoLikedThat-/terms.html)
  * [Support](https://arturo918.github.io/WhoLikedThat-/support.html)

---

## 🚀 Local Development Setup

### Prerequisites
* Node.js (v18+)
* npm or pnpm

### Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/arturo918/WhoLikedThat-.git](https://github.com/arturo918/WhoLikedThat-.git)
   cd WhoLikedThat-
