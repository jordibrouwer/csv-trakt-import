# hdtv-to-trakt-exporter 📺✈️🍿

A lightweight Python utility designed to help former **hdtv app** users migrate their watched TV show history over to **Trakt.tv**. 

Since hdtv abruptly shut down, many of us lost access to our carefully curated watchlists. If you managed to grab a backup of your data in a basic CSV format before the lights went out, this script will automatically fetch the required **TMDB IDs**, set the content type to **'show'**, and format everything perfectly for a seamless Trakt import.

---

## 🚀 Features

* **Auto-Matching:** Automatically searches The Movie Database (TMDB) API to find unique show identifiers.
* **Trakt-Ready Formatting:** Hardcodes the type to `'show'` and maps IDs into the precise headers Trakt's import tool expects (`tmdb`, `imdb`, `type`, `title`, `watched_at`).
* **Smart Backups:** Fetches IMDb IDs as a fallback option when available.
* **Rate-Limit Friendly:** Built-in sleep intervals to respect TMDB API limits.

---

## 🛠️ Prerequisites

Before running the script, make sure you have:

1. **Python 3.x** installed on your system.
2. The `requests` library installed. You can grab it via terminal:
   ```bash
   pip3 install requests
