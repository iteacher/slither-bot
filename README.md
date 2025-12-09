# Hoobs Slither Mod

A **Slither.io game mod** that enhances your gameplay with modern features including a glassmorphic UI, auto-eat functionality, collision avoidance, and mouse scroll zoom.

![Version](https://img.shields.io/badge/version-0.9.12-blue)
![Platform](https://img.shields.io/badge/platform-Tampermonkey-green)
![Game](https://img.shields.io/badge/game-Slither.io-orange)

## Features

- 🎨 **Modern Glassmorphic UI** - Clean, modern interface design
- 🍽️ **Auto-Eat** - Automatically navigate towards food
- 🛡️ **Collision Avoidance** - Smart threat detection and avoidance system
- 🔍 **Mouse Scroll Zoom** - Zoom in/out using your mouse scroll wheel
- 📡 **Threat Radar** - Real-time polar heatmap showing nearby threats
- 🎯 **Customizable Cursor** - Adjust cursor size and opacity
- 🎛️ **Adjustable Settings** - Fine-tune radar distance, avoidance sensitivity, and more
- 💾 **Persistent Settings** - Your preferences are saved between sessions
- 🖼️ **Custom Background** - Remove default background or set custom colors

## Installation

### Prerequisites

You need **Tampermonkey** installed in your browser. Tampermonkey is a popular browser extension that acts as a userscript manager, allowing you to install and run custom scripts to enhance websites.

#### Install Tampermonkey

| Browser | Installation Link |
|---------|------------------|
| Chrome | [Chrome Web Store](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) |
| Firefox | [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/) |
| Edge | [Microsoft Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpaadaobahmlepeloendndfphd) |
| Safari | [Mac App Store](https://apps.apple.com/app/tampermonkey/id1482490089) |
| Opera | [Opera Add-ons](https://addons.opera.com/en/extensions/details/tampermonkey-beta/) |

### Installing the Mod

1. **Install Tampermonkey** in your browser (see links above)
2. **Click the Tampermonkey icon** in your browser toolbar
3. **Select "Create a new script..."**
4. **Delete the template code** that appears
5. **Copy the entire contents** of `mod.js` and paste it into the editor
6. **Press Ctrl+S** (or Cmd+S on Mac) to save
7. **Navigate to [slither.io](http://slither.io)** and enjoy!

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Tab` | Open/Close Settings Panel |
| `Esc` | Quick Respawn |
| `Q` | Quit to Menu |
| `Z` | Restore Default Zoom |
| `E` | Toggle Auto-Eat |
| `C` | Toggle Auto-Avoid |

## Settings

Access the settings panel by pressing `Tab` or clicking the **Settings** button on the main menu.

### UI Settings
- **Default BG** - Toggle the default game background
- **Cursor Size** - Adjust the crosshair cursor size (8-64px)
- **Cursor Opacity** - Adjust cursor transparency (0.1-1.0)

### Radar Settings
- **Radar Distance** - Detection range for the threat radar (outer circle)
- **Avoid Distance** - Collision avoidance trigger range (inner circle)
- **Sectors** - Angular resolution of the radar (8-64)
- **Rings** - Radial resolution of the radar (3-12)
- **Heat Decay** - How quickly threat indicators fade
- **Food Range** - Search radius multiplier for auto-eat

### Overlays
- **Collision** - Show collision detection overlay
- **Feeding** - Show food paths and targets
- **Radar** - Show the threat heatmap radar

### Stance Toggles
- **Auto-Avoid** - Enable automatic collision avoidance
- **Auto-Eat** - Enable automatic food seeking

## How It Works

### Threat Radar
The mod uses a polar coordinate heatmap system to detect and visualize nearby threats. Snake heads are weighted heavily as primary threats, while body segments contribute less heat. The radar uses configurable sectors (angular divisions) and rings (radial divisions) for precise threat localization.

### Auto-Avoid
When enabled, the mod analyzes the threat heatmap and calculates safe steering vectors to avoid collisions. The system predicts enemy snake movements and adjusts your trajectory accordingly.

### Auto-Eat
The auto-eat feature uses a TSP (Traveling Salesman Problem) approach to efficiently route through nearby food, prioritizing high-value targets while respecting threat zones.

## Security Note

⚠️ **Important**: Only install userscripts from sources you trust. Userscripts have access to webpage content and can potentially be malicious. This mod is open source - feel free to review the code before installing.

## Author

**minigem.uk**

## License

This project is provided as-is for educational and entertainment purposes.

---

*Enjoy dominating the leaderboard! 🐍*
