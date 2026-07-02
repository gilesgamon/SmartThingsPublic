# FIFA World Cup 2026 - Live Tracker

A beautiful, live-updating visualization for tracking the FIFA World Cup 2026 tournament.

## 🚀 Quick Start

### Option 1: Run Local Server (Recommended)

The easiest way to run locally:

```bash
# Navigate to the folder containing index.html
cd /path/to/worldcup-tracker

# Python 3 (most common)
python3 serve.py

# Or manually with Python 3
python3 -m http.server 8000

# Or with Node.js
npx http-server
```

Then open: `http://localhost:8000`

### Option 2: Use VS Code Live Server

1. Install "Live Server" extension in VS Code
2. Right-click `index.html` → "Open with Live Server"

### Option 3: Deploy to GitHub Pages

See `DEPLOYMENT.md` for full instructions. Your tracker will be live at:
```
https://gilesgamon.github.io/SmartThingsPublic/
```

## ⚠️ Important: Don't Open File Directly

**Don't double-click the HTML file!** Modern browsers block API calls from `file://` URLs for security.

You **must** serve it via HTTP using one of the methods above.

## ✨ Features

- **Live Data Updates**: Auto-refreshes every 30 seconds
- **Group Stage Wheel**: All 12 groups (A-L) with 48 teams
- **Match Countdown**: Shows time until kickoff for upcoming matches
- **Live Match Tracking**: Real-time scores with pulsing indicators
- **Match Details**: All 104 matches with formatted dates and stadium info
- **Responsive Design**: Works on desktop, tablet, and mobile

## 📱 Views

### Group Stage
- View all 12 groups with team standings
- See points (Pts), goals for (GF), and goals against (GA)
- Real-time statistics during tournament

### All Matches
- Browse all 104 tournament matches
- Formatted dates: "Wed, Jun 11, 1:00 PM"
- Countdown timers: "⏰ Kickoff in 2 days, 5h"
- Stadium locations with 📍 emoji

### Live Matches
- Filter to show only currently playing matches
- Live score updates with match time
- Pulsing red indicator for active games

## 🔌 API

Uses the free, open-source [FIFA World Cup 2026 API](https://worldcup26.ir):
- No authentication required
- Real-time updates during tournament
- Complete data for teams, groups, matches, and stadiums

## 🛠️ Technical Details

- **Pure HTML/CSS/JavaScript** - No frameworks, no build process
- **Zero dependencies** - Just open and run
- **Auto-refresh** - Every 30 seconds
- **CORS-enabled API** - Works from any domain
- **Responsive grid layout** - Adapts to all screen sizes

## 📦 Files

- `index.html` - Main tracker (GitHub Pages ready)
- `worldcup-wheel.html` - Standalone version
- `serve.py` - Quick local server script
- `DEPLOYMENT.md` - Deployment guide
- `WORLDCUP_README.md` - This file

## 🌐 Browser Compatibility

- ✅ Chrome/Edge 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Opera 76+

## 🐛 Troubleshooting

### "Unable to connect to FIFA World Cup API"

**Cause**: You're opening the file directly (`file://` protocol)

**Solution**: Serve via HTTP using one of the methods above

### API Rate Limits

The free API allows 120 requests per minute. The tracker makes 4 requests every 30 seconds (8 per minute), so you're well within limits.

## 📄 License

This is a standalone visualization tool using the public FIFA World Cup 2026 API.
