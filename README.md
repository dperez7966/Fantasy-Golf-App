# ⛳ Fantasy Golf League Tracker

A live fantasy golf league tracking app with real-time ESPN leaderboard integration.

## 🎯 Features

- **📊 Live Scores** - Real-time leaderboard from ESPN.com
- **🏆 Season Standings** - Track all players across the entire season
- **📋 Picks Used** - See which golfers each player has already used
- **📜 Pick History** - Filter by player or tournament
- **📱 Mobile Friendly** - Works great on phones and tablets

## 🚀 Quick Start

Just visit the site - no installation or uploads needed! Data is embedded and updates automatically.

**Live Site:** [Your GitHub Pages URL will go here]

## 👥 League Members

- Mike
- Gordo
- Kyle
- Craig
- Phil
- Todd
- Rahul
- Andrew
- Dan

## 📖 How to Use

### This Week Tab
View current tournament info, purse, and dates. See who's leading the season.

### 🔴 Live Tab
- Click "Load Live Scores" to fetch current tournament standings from ESPN
- Auto-refreshes every 3 minutes
- Shows position, score, holes completed, and projected earnings for your picks

### Picks Used Tab
- See which golfers each player has used this season
- Filter by individual player
- Helps avoid picking golfers already used

### Standings Tab
- Full season leaderboard
- Week-by-week breakdown (scroll horizontally)
- Sorted by total earnings

### History Tab
- All picks from all tournaments
- Filter by player and/or tournament
- Shows earnings for each pick

## 🔄 Updating Data

**For League Administrator:**

To update picks and results after each tournament:

1. Go to your repository on GitHub
2. Click on `index.html`
3. Click the pencil icon (✏️) to edit
4. Update the `EMBEDDED_DATA` section with new picks/results
5. Commit changes
6. Site updates automatically in 1-2 minutes

**Data Format:**
```javascript
const EMBEDDED_DATA = {
  "historical": [
    {
      "Player": "Dan",
      "Tournament": "The American Express",
      "Pick": "Nick Taylor",
      "Results": 0
    }
    // ... more picks
  ],
  "tournaments": [
    {
      "Tournament Name": "The American Express",
      "Tournament Start Date": "2026-01-22T00:00:00",
      "Tournament End Date": "2026-01-25T00:00:00",
      "Tournament Purse": 8800000
    }
    // ... more tournaments
  ]
}
```

## 🛠️ Tech Stack

- **React 18** - UI framework
- **Tailwind CSS** - Styling
- **ESPN Web Scraping** - Live scores
- **GitHub Pages** - Free hosting

## 📝 Rules

- Players cannot pick the same golfer twice in a season
- Pick order based on previous week's results (lowest to highest)
- Lowest earners pick first (snake draft style)

## 🐛 Troubleshooting

**Live scores not loading?**
- CORS proxy may be temporarily down
- Try refreshing the page
- ESPN might have changed their website structure

**Dates showing incorrectly?**
- Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)

**Currency showing as "0$0"?**
- Hard refresh your browser

## 📧 Contact

Questions? Contact the league administrator.

## 📄 License

Personal use for fantasy golf league.
