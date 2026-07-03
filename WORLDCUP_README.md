# FIFA World Cup 2026 - Live Tracker Wheel

A beautiful, live-updating visualization for tracking the FIFA World Cup 2026 tournament.

## Features

- **Live Data Updates**: Auto-refreshes every 30 seconds to show real-time match scores
- **Group Stage Wheel**: Circular grid layout displaying all 12 groups (A-L) with 48 teams
- **Live Match Tracking**: View ongoing matches with live score updates
- **Match Details**: See all 104 matches with scores, times, and stadium information
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Modern UI**: Beautiful gradient design with smooth animations

## How to Use

1. Simply open `worldcup-wheel.html` in any modern web browser
2. No installation or dependencies required
3. The app will automatically fetch live data from the FIFA World Cup 2026 API

## Views

### Group Stage
- View all 12 groups with team standings
- See points (Pts), goals for (GF), and goals against (GA)
- Teams are organized by group with real-time statistics

### All Matches
- Browse all 104 tournament matches
- View scores, dates, and stadium locations
- See match status (Upcoming, Live, Finished)

### Live Matches
- Filter to show only currently playing matches
- Live score updates with match time
- Pulsing indicator for active games

## API

This tracker uses the free, open-source [FIFA World Cup 2026 API](https://worldcup26.ir):
- No authentication required for read access
- Real-time updates during tournament
- Complete data for all teams, groups, matches, and stadiums

**Important:** Match times are provided in **stadium local time**, not a single global timezone:
- Games in **Eastern** stadiums (Toronto, New York, Miami, etc): EDT (UTC-4) / EST (UTC-5)
- Games in **Central** stadiums (Mexico City, Dallas, Houston, etc): CDT (UTC-5) / CST (UTC-6)
- Games in **Western** stadiums (LA, Seattle, Vancouver, etc): PDT (UTC-7) / PST (UTC-8)

The app automatically converts each match time to your browser's local timezone based on the stadium location.

## Technical Details

- Pure HTML/CSS/JavaScript (no frameworks required)
- Fetches data from: `https://worldcup26.ir`
- Auto-refresh: Every 30 seconds
- Responsive grid layout
- Modern glassmorphism design

## Browser Compatibility

Works with all modern browsers:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Opera 76+

## License

This is a standalone visualization tool using the public FIFA World Cup 2026 API.
