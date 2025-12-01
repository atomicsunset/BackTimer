# Atomation BackTimer

A precision broadcast timing tool for radio professionals. Calculate exactly when to start your intro and commercial segments to hit your hard out (radio live time) perfectly.

## Features

- **Precision Timing** - Millisecond-accurate countdown with 30fps updates
- **Visual Alerts** - Color-coded warnings at 5 minutes, 3 minutes, and final countdown
- **Segment Management** - Add multiple intro/commercial segments with custom names and durations
- **Real-time Clock** - Live current time display
- **Smart Calculations** - Automatically handles midnight wraparound
- **Dark Modern UI** - Clean, professional interface built with Tailwind CSS
- **No Installation** - Single HTML file, runs in any modern browser
- **Offline Capable** - Uses CDN resources but can work offline once loaded

## How It Works

1. **Set Your Hard Out** - Enter the radio live time (the exact moment you need to be live on air)
2. **Add Segments** - Input your intro and commercial segments with their durations
3. **Get Start Time** - BackTimer calculates exactly when to start playing your intro
4. **Watch Countdown** - Visual alerts guide you through the timing:
   - **ON STANDBY** (>5 mins) - Waiting mode
   - **5 MIN WARNING** (3-5 mins) - Yellow alert, prepare for intro
   - **3 MIN WARNING** (1.5-3 mins) - Orange alert, get ready
   - **ACTIVE COUNTDOWN** (0-90s) - Live countdown with milliseconds
   - **GO GO GO** (0 to -5s) - Green flash, start your intro now!
   - **BROADCAST UNDERWAY** (<-5s) - You're live

## Usage

### Quick Start

1. Open `index.html` in your web browser
2. Enter your radio live time (hard out) in the top section
3. Add your segments:
   - Give each segment a name (e.g., "Station ID", "Commercial Break")
   - Enter the duration in minutes and seconds
   - Click "Add" or press Enter
4. Watch the **Start Intro At** time - that's when you need to begin
5. Monitor the alert box for visual timing cues

### Example Scenario

**Radio Live Time:** 12:00:00 PM

**Segments:**
- Station ID: 0:30
- Commercial 1: 1:00
- Commercial 2: 1:00
- Show Intro: 2:30

**Total Content:** 00:05:00

**Start Intro At:** 11:55:00 AM

BackTimer will show you exactly when to hit play, and guide you with visual alerts as you approach the hard out.

## Use Cases

- **Radio Broadcasting** - Hit hard outs perfectly every time
- **Podcasting** - Time your intro/outro segments precisely
- **Live Events** - Countdown to exact start times
- **Production** - Coordinate timed content delivery
- **Training** - Teach broadcast timing techniques

## Technical Details

- **Update Frequency:** 30fps for smooth countdown display
- **Precision:** Millisecond-accurate calculations
- **Framework:** Vanilla JavaScript with Tailwind CSS
- **Fonts:** Inter (UI) and JetBrains Mono (monospace numbers)
- **Icons:** Font Awesome 6.0
- **Browser Support:** Any modern browser (Chrome, Firefox, Safari, Edge)

## Keyboard Shortcuts

- **Enter** - Add segment (when in duration input fields)
- **Tab** - Navigate between input fields

## Tips for Best Results

1. **Test Your Timing** - Run a practice session before going live
2. **Account for Delays** - Add a small buffer if your playback system has latency
3. **Use Descriptive Names** - Label segments clearly for quick reference
4. **Watch the Countdown** - The final 10-second flash is your last warning
5. **Trust the Timer** - The math is precise, hit GO when it flashes green

## Customization

The HTML file is self-contained and easy to customize:

- **Colors:** Edit the Tailwind CSS classes in the HTML
- **Alert Timings:** Modify the `checkAlerts()` function thresholds
- **Update Frequency:** Change `setInterval(updateWallClock, 33)` (33ms = 30fps)
- **Fonts:** Replace the Google Fonts import URL

## Browser Compatibility

Works in all modern browsers:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

Requires JavaScript enabled.

## File Structure

```
BackTimer/
├── index.html          # Complete application (single file)
└── README.md           # This file
```

## Support

For issues or suggestions, create an issue on the GitHub repository.

## License

MIT License - See LICENSE file for details

## Credits

- Created by Atomation
- Built with Tailwind CSS
- Icons by Font Awesome

---

**Made for broadcasters, by a broadcaster.**