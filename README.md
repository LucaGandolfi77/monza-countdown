# 🛼 Monza Precision Team - Countdown to World Championships

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

A beautiful interactive countdown application for the Monza Precision Team on their journey to the 2025 World Championships.

[Demo](#demo) • [Features](#features) • [Installation](#installation) • [Usage](#usage) • [Contributing](#contributing)

</div>

---

## 📋 Table of Contents

- [Overview](#overview)
- [Demo](#demo)
- [Features](#features)
- [Technologies](#technologies)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Customization](#customization)
- [Browser Support](#browser-support)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## 🎯 Overview

This mobile-first application is an interactive countdown calendar designed for the Monza Precision Team. Each day of October 2025, team members can open a digital "box" to reveal a unique motivational quote, creating an engaging experience on the journey to the World Championships.

### 🌟 Highlights

- ✨ **Animated Glitter Effects** - Sparkling particles and twinkling stars
- 📱 **Mobile-First Design** - Optimized for iPhone and mobile devices
- 🎨 **Smooth Animations** - Elegant transitions and visual feedback
- 🔒 **Smart Unlocking System** - Boxes open only on the correct day
- 💾 **Local Persistence** - Remembers which boxes have been opened
- 🇮🇹 **Italian Interface** - UI and motivational quotes in Italian

---

## 🎬 Demo

![App Screenshot](https://via.placeholder.com/800x600/667eea/ffffff?text=Monza+Precision+Team+Countdown)

### Features in Action

- **Locked Boxes** (gray) - Future dates not yet available
- **Available Boxes** (white/purple) - Ready to be opened
- **Opened Boxes** (green with ✓) - Already viewed

---

## ✨ Features

### 🎨 Design & UI

- **Gradient Background** - Elegant purple/blue gradient background
- **Glitter Effects** - 50+ animated particles for a magical effect
- **Responsive Grid** - Automatic adaptation to all screen sizes
- **Smooth Animations** - Hover, pulse, and shimmer effects
- **Modal Pop-ups** - Elegant modal windows with daily quotes

### 🔧 Technical Features

- **Date-Based Unlocking** - Unlocking system based on actual date
- **Session Storage** - Saving opened boxes state
- **Touch-Optimized** - Interactions perfectly optimized for touch
- **No Dependencies** - Zero external dependencies, pure vanilla JavaScript
- **Single File** - Everything contained in one portable HTML file

### 📝 Content

- **30 Motivational Quotes** - A unique quote for each day
- **Skating Theme** - Quotes inspired by roller skating and sports
- **Italian Localization** - Fully translated interface

---

## 🛠 Technologies

This project is built using pure web technologies:

- **HTML5** - Semantic structure
- **CSS3** - Advanced styling with animations and gradients
- **Vanilla JavaScript** - Application logic without frameworks
- **Session Storage API** - Local data persistence

---

## 📥 Installation

### Method 1: Direct Download

1. Download the `index.html` file
2. Open the file directly in your browser

```bash
# On macOS/Linux
open index.html

# On Windows
start index.html
```

### Method 2: Clone Repository

```bash
# Clone the repository
git clone https://github.com/yourusername/monza-countdown.git

# Enter the directory
cd monza-countdown

# Open the file
open index.html
```

### Method 3: Local Web Server

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (with http-server)
npx http-server

# Then open http://localhost:8000 in your browser
```

---

## 🚀 Usage

### Basic Usage

1. **Open the application** - Load `index.html` in your browser
2. **View the calendar** - You'll see 30 boxes numbered from 1 to 30
3. **Click on an available box** - Only today's or past dates are clickable
4. **Read the motivational quote** - Each day has a unique quote
5. **Close the modal** - The box will remain marked as opened

### Box States

| State | Color | Description |
|-------|--------|-------------|
| 🔒 Locked | Gray | Future date - not yet available |
| ✅ Available | White/Purple | Today or past date - ready to be opened |
| ✓ Opened | Green | Already opened - shows a checkmark |

### Mobile Usage

The app is optimized for mobile devices:

- **Touch Friendly** - Sufficiently large tap areas
- **Responsive** - Automatically adapts to screen
- **Apple PWA Ready** - Can be added to home screen on iOS

```html
<!-- To add to iOS home screen -->
<!-- The app is already configured with necessary meta tags -->
```

---

## 📁 Project Structure

```
monza-countdown/
│
├── index.html              # Main application file
│   ├── <style>            # Inline CSS with animations
│   ├── <body>             # HTML structure
│   └── <script>           # JavaScript for logic
│
├── README.md              # This file
└── LICENSE                # MIT License
```

### Key Components

```javascript
// Key functions in the code
createGlitter()           // Creates the glitter effect
initCalendar()            // Initializes the calendar
openBox(day)              // Opens a specific box
closeModal()              // Closes the modal
getOpenedBoxes()          // Retrieves opened boxes
markBoxAsOpened(day)      // Marks a box as opened
```

---

## 🎨 Customization

### Modify Colors

Find the CSS section and modify the gradients:

```css
/* Main background */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Opened boxes */
background: linear-gradient(135deg, #11998e 0%, #38ef7d 100%);
```

### Add/Modify Quotes

Edit the `quotes` array in JavaScript:

```javascript
const quotes = [
    "Your new motivational quote here!",
    "Another inspirational quote...",
    // ... add 30 total quotes
];
```

### Change Month/Year

Modify the `OCTOBER_2025` object:

```javascript
const OCTOBER_2025 = {
    year: 2025,    // Desired year
    month: 9       // Month (0-indexed: 0=Jan, 9=Oct)
};
```

### Modify Number of Days

Change the loop in `initCalendar()`:

```javascript
for (let day = 1; day <= 30; day++) {  // Change 30 to desired number
    // ...
}
```

---

## 🌐 Browser Support

| Browser | Minimum Version |
|---------|-----------------|
| Chrome | 90+ |
| Safari | 14+ |
| Firefox | 88+ |
| Edge | 90+ |
| iOS Safari | 14+ |
| Chrome Mobile | 90+ |

### Feature Compatibility

- ✅ CSS Grid
- ✅ CSS Animations
- ✅ Flexbox
- ✅ Session Storage
- ✅ ES6+ JavaScript
- ✅ Mobile Touch Events

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

### How to Contribute

1. **Fork the project**
   ```bash
   git fork https://github.com/yourusername/monza-countdown.git
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```

3. **Commit your changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```

4. **Push to the branch**
   ```bash
   git push origin feature/AmazingFeature
   ```

5. **Open a Pull Request**

### Guidelines

- Keep code simple and readable
- Comment complex functions
- Test on mobile devices
- Ensure animations are smooth
- Maintain browser compatibility

---

## 📝 Roadmap

- [ ] Add sounds when opening a box
- [ ] Implement social sharing of quotes
- [ ] Add dark/light mode
- [ ] Create full PWA version with offline support
- [ ] Add box opening statistics
- [ ] Implement achievement/badge system
- [ ] Add confetti animations on opening

---

## 📄 License

This project is released under the MIT License. See the `LICENSE` file for more details.

```
MIT License

Copyright (c) 2025 Monza Precision Team

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

---

## 👥 Contact

**Monza Precision Team**

- Website: [monzaprecisionteam.it](https://monzaprecisionteam.it)
- Email: info@monzaprecisionteam.it
- Instagram: [@monzaprecisionteam](https://instagram.com/monzaprecisionteam)

---

## 🙏 Acknowledgments

- Thanks to the entire Monza Precision Team for the inspiration
- Motivational quotes inspired by the roller skating community
- Design inspired by modern mobile-first applications

---

## ⭐ Support

If this project was helpful to you, consider:

- ⭐ Starring the repository
- 🐛 Reporting bugs or issues
- 💡 Suggesting new features
- 🔄 Sharing with other teams

---

<div align="center">

**Made with ❤️ for the Monza Precision Team**

🛼 To the 2025 World Championships! 🛼

[⬆ Back to top](#-monza-precision-team---countdown-to-world-championships)

</div>