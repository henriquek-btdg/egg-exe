# egg.exe

![Game](https://img.shields.io/badge/game-interactive%20fiction-green)
![Twine](https://img.shields.io/badge/made%20with-Twine-orange)
![Status](https://img.shields.io/badge/status-released-blue)
![License](https://img.shields.io/github/license/henriquek-btdg/egg-exe)
![GitHub repo size](https://img.shields.io/github/repo-size/henriquek-btdg/egg-exe)
![GitHub stars](https://img.shields.io/github/stars/henriquek-btdg/egg-exe?style=social)
![GitHub forks](https://img.shields.io/github/forks/henriquek-btdg/egg-exe?style=social)
![GitHub last commit](https://img.shields.io/github/last-commit/henriquek-btdg/egg-exe)

An experimental interactive narrative game about memories, choices, and the weight we carry.


Made in less than 1 week for a Game Jam with the theme: **"What is inside that egg?"**

This game was made with the objective to further develop skills in
HTML, CSS and Javascript in a fun way.

## ⚠️ Content Warnings

This game contains:
- Themes related to mental health, including references to suicide and self-harm
- Flashing visual effects that may cause discomfort for people with photosensitive epilepsy
- Content that may be disturbing for some players

**If you or someone you know needs help:**
- 🇧🇷 Brazil: CVV - **188** (24/7, free) | Chat: [www.cvv.org.br](https://www.cvv.org.br)
- 🌍 International: [findahelpline.com](https://findahelpline.com)

## 🎮 How to Play

### Play Online:
[**► PLAY NOW**](https://battledawg.itch.io/egg-exe)

### Play Locally:
1. Download or clone this repository
2. Open `index.html` in your web browser
3. Make sure to allow audio autoplay when prompted

## 📖 About

**egg.exe** is a psychological interactive fiction game about cataloging memories. You are an operator processing "eggs" that represent memories, each carrying different emotional weight. Your choices determine not only the ending, but your very capacity to continue processing memories.

Through a retro terminal interface, you'll face 13 eggs across 5 days. Each decision matters:
- **Incubate** memories to keep them
- **Neutralize** them to let go
- **Observe** to understand them better (limited uses)

But be careful—your analysis capacity is limited, and wrong choices can leave you operating blind.

## ✨ Features

- **Branching narrative** with 5 distinct endings
- **Consequence-driven mechanics**: choices affect your gameplay capacity
- **Retro terminal aesthetic** with glitch effects and ASCII art
- **Dynamic soundscape** with reactive audio feedback
- **Capacity management system** that forces strategic thinking
- **Randomized outcomes** based on your emotional balance (light vs shadow)

## 🎨 Endings

The game features multiple endings based on your choices:
- **"Guardião de Memórias" (Memory Guardian)** - Light path
- **"Livre" (Free)** - Secret ending
- **"Mais Um Dia" (One More Day)** - Neutral/Incubate path
- **"Recomeço" (New Beginning)** - Neutral/Neutralize path
- **"O Peso do Silêncio" (The Weight of Silence)** - Dark path

## 🛠️ Technical Details

- **Engine:** Twine (Harlowe 3.3.9)
- **Audio:** HAL (Harlowe Audio Library v2.3.0)
- **Custom CSS** for terminal/retro aesthetic
- **JavaScript** for flickering effects and UI controls
- **HTML5 Audio** for dynamic sound design

### Game Mechanics:
- **Capacity System:** Start with 6 analysis points, gain/lose based on choices
- **Light/Shadow Balance:** Affects random event outcomes
- **Progressive Difficulty:** System deteriorates from Day 3 onwards
- **Observation Lock:** Can't observe eggs without capacity

## 📁 Repository Structure
```
egg-exe/
├── index.html          # Main game file (exported from Twine)
├── README.md           # This file
├── src/                    # Source code
│   ├── egg.twee           # Twine source file
│   ├── story.js           # Custom JavaScript
│   └── style.css          # Custom CSS
└── audio/              # Sound effects and music
    ├── ambienceSound.mp3
    ├── ganhoCapacidade.mp3
    ├── perdaCapacidade.mp3
    ├── glitch.mp3
    ├── alarmeCritico.mp3
    └── cliqueBotao.mp3
```

## 🎵 Audio Credits

With a Stamp by Twin Musicom is licensed under a Creative Commons Attribution 4.0 license. https://creativecommons.org/licenses/by/4.0/

Artist: http://www.twinmusicom.org/

## 🕹️ Controls

- **Click/Tap** on highlighted text to make choices
- **Press the button** on the lower right corner to toggle screen flicker effect (accessibility)
- **Undo/Redo buttons** in corner (use cautiously - may affect experience)

## 🐛 Known Issues

- Some browsers may block audio autoplay on first load (click anywhere to enable)
- Screen flicker effect can be disabled via toggle button for accessibility
- Best experienced on desktop browsers (Chrome, Firefox, Safari)

## 🚀 Future Updates

- [ ] Additional language support (currently available in portuguese)
- [ ] More endings/branches
- [ ] Extended Day 5 content
- [ ] Accessibility options menu

## 🔧 Development

### Prerequisites

- [Twine 2](https://twinery.org/) (for editing)
- Modern web browser (for testing)
- Text editor (VS Code, Sublime, etc.)

### Setting Up

1. **Clone the repository:**
```bash
git clone https://github.com/your-username/egg-exe.git
cd egg-exe
```

2. **Import to Twine:**
   - Open Twine
   - Click "Import From File"
   - Select `src/egg.twee` (or `index.html`)

3. **Edit the game:**
   - Passages: Edit in Twine interface
   - CSS: Edit `src/style.css` OR Story → Stylesheet in Twine
   - JavaScript: Edit `src/story.js` OR Story → JavaScript in Twine

4. **Test:**
   - In Twine: Click "Play" button
   - OR open `index.html` in browser

### Building

**From Twine:**
1. Story menu → "Publish to File"
2. Save as `index.html` (overwrites old version)

**From Command Line (optional - using Tweego):**
```bash
tweego src/egg.twee -o index.html
```

### File Descriptions

#### `src/egg.twee`
Main story file containing all passages, variables, and narrative logic.

#### `src/style.css`
Custom styling including:
- Terminal aesthetic (green text, scanlines, flicker)
- Animations (glitch, pulse, shake, blink)
- Button styles
- Accessibility options

#### `src/story.js`
Custom JavaScript for:
- Flicker toggle system
- Random event handling
- UI enhancements
- Audio management (if not using HAL)

#### `audio/`
All game sound effects:
- `ambienceSound.mp3` - Background music/ambience
- `ganhoCapacidade.mp3` - Capacity gain sound
- `perdaCapacidade.mp3` - Capacity loss sound
- `glitch.mp3` - System glitch effect
- `alarmeCritico.mp3` - Critical alarm
- `cliqueBotao.mp3` - Button click sound

## 🎨 Customization

### Changing Colors

Edit `src/style.css`:
```css
/* Main terminal color */
color: #00ff41;  /* Change this hex code */

/* Background */
background-color: #0a0a0a;  /* Change this */
```

### Adding New Sounds

1. Add `.mp3` file to `audio/` folder
2. In Twine, edit `StoryInit` passage (or HAL.tracks):
```
(track: 'newSound', './audio/newSound.mp3')
```
3. Use in passages:
```
(track: 'newSound', 'play')
```

### Adjusting Capacity Balance

Edit `src/egg.twee`, find passage `Login`:
```
(set: $capacidade to 6)  /* Change starting capacity */
```

## 🤝 Contributing

This is a personal project, but if you'd like to:
- **Report bugs:** Open an issue
- **Suggest features:** Open an issue with "enhancement" tag
- **Fork & modify:** Feel free! Just credit the original

### How to Contribute

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes
4. Test thoroughly
5. Commit: `git commit -m "Add feature"`
6. Push: `git push origin feature-name`
7. Open a Pull Request


## 🙏 Credits

**Game Design & Development:** Henrique Karez

**Tools Used:**
- Twine by Chris Klimas
- Harlowe story format
- HAL (Harlowe Audio Library) by Chapel

## 💬 Feedback

Found a bug? Have suggestions? Feel free to:
- Open an issue on GitHub
- Contact me at henriquekarez@gmail.com
- Leave a comment on https://battledawg.itch.io/

## 🔗 Links

- **Play on Itch.io:** [https://battledawg.itch.io/egg-exe]
- **Developer:** [https://linktr.ee/henriquekarez]

---
**If you enjoyed this project, consider starring the repo!**


Made in Twine | Play responsibly | Take care of your mental health
