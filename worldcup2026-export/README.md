# FIFA World Cup 2026 Live Tracker 🏆

A beautiful, live-updating circular "wheel" visualization for tracking the FIFA World Cup 2026, featuring a radial tournament bracket with country flags and real-time match data.

![Version](https://img.shields.io/badge/version-1.5.3-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## 🌟 Features

- **Live Match Updates**: Real-time scores and match status from the FIFA API
- **Timezone Selector**: 🌍 Choose your timezone from 35+ options or auto-detect
- **Circular Bracket Design**: Radial layout showing progression from Round of 32 to the Final
- **Horizontal Semi-Finals**: Semi-final matches displayed horizontally for clarity
- **Country Flags**: Visual spheres with national flags for each team
- **Match Information**: 
  - Live matches display current score with 🔴 LIVE indicator
  - Upcoming matches show date/time in your selected timezone
  - Finished matches show final scores
- **Visual Progression**: Green connecting lines show team advancement through rounds
- **Winner/Eliminated States**: Visual indicators for teams that won or lost
- **Auto-refresh**: Data updates automatically every minute
- **Responsive Design**: Works on all screen sizes

## 🚀 Live Demo

**Visit:** [https://gilesgamon.github.io/WorldCup2026/](https://gilesgamon.github.io/WorldCup2026/)

## 🌍 Timezone Features

- **Auto-detect** your browser's timezone
- **35+ timezone options** organized by region:
  - Americas (PT, MT, CT, ET, Brazil, Argentina, Mexico)
  - Europe (London, Paris, Berlin, Madrid, Rome, Moscow)
  - Asia (Dubai, India, Bangkok, China, Tokyo, Seoul)
  - Pacific (Sydney, Melbourne, Auckland)
  - Africa (Cairo, Lagos, Johannesburg)
- **Instant updates** when you change timezone
- Selector located at bottom-center of the screen

## 🛠️ Local Development

Due to CORS restrictions, serve via HTTP server:

```bash
# Using the included Python script (recommended)
python3 serve.py

# Or use Python's built-in server
python3 -m http.server 8000

# Then open: http://localhost:8000
```

## 📦 Installation

Just clone and open:

```bash
git clone https://github.com/gilesgamon/WorldCup2026.git
cd WorldCup2026
python3 serve.py
```

## 🔌 API Integration

Uses the free FIFA World Cup 2026 API at `https://worldcup26.ir`:

- `/get/games` - Match schedules and results
- `/get/teams` - Team information and flags
- `/get/groups` - Group stage standings
- `/get/stadiums` - Venue information

## 📋 Files

- `index.html` - Main application (single-file, no build required)
- `serve.py` - Convenience script for local development
- `DEPLOYMENT.md` - Deployment options guide

## 🎨 Technical Details

- **Canvas-based rendering** for precise bracket visualization
- **Timezone conversion** using JavaScript Intl API
- **No dependencies** - pure HTML/CSS/JavaScript
- **Single file deployment** - just `index.html`

## 📝 Version History

- **v1.5.3** - Move timezone selector to bottom-center
- **v1.5.2** - Remove timezone abbreviation from match times
- **v1.5.1** - Add timezone selector dropdown with 35+ options
- **v1.5.0** - Add automatic timezone detection
- **v1.4.3** - Fix semi-final orientation to horizontal
- **v1.4.1** - Fix bracket visual alignment with cascading reordering
- **v1.3.0** - Implement R32 match reordering by destination
- **v1.2.2** - Migrate from SVG to Canvas for better control
- **v1.0.0** - Initial release

## 🤝 Contributing

Contributions are welcome! Feel free to:

- Report bugs
- Suggest new features
- Submit pull requests

## 📄 License

MIT License - feel free to use this for your own projects!

## 🙏 Acknowledgments

- FIFA World Cup 2026 API: [worldcup26.ir](https://worldcup26.ir)
- Flag images: [flagcdn.com](https://flagcdn.com)

---

**Made with ⚽ for FIFA World Cup 2026**
