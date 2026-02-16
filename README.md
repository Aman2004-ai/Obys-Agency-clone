# Obys Agency Clone

A modern, animated web design agency portfolio website built with vanilla HTML, CSS, and JavaScript. This project showcases smooth scrolling animations, interactive cursor effects, and creative visual enhancements.

![Obys Agency](https://img.shields.io/badge/Design-Modern%20Agency-brightgreen) ![Status](https://img.shields.io/badge/Status-Active-success)

---

## 🎨 Project Overview

**Obys Agency Clone** is a pixel-perfect recreation of the award-winning [Obys Agency](https://obys.agency/) website. It demonstrates modern web design techniques including:

- **Smooth Scrolling:** Locomotive Scroll for buttery-smooth scroll animations
- **Advanced Animations:** GSAP (GreenSock Animation Platform) for dynamic effects
- **Interactive Effects:** Shery.js for creative WebGL-based image distortions
- **Custom Cursor:** Mouse-following cursor with magnetic interactions
- **Responsive Design:** Mobile-first approach with smooth performance

---

## 🚀 Features

✨ **Smooth Scroll Experience**
- Locomotive Scroll integration with parallax effects
- ScrollTrigger synchronization for scroll-based animations

🎬 **Loading Animation**
- Animated number counter in loader
- Smooth text transitions and staggered animations
- Custom font effects with opacity transitions

🖱️ **Interactive Cursor**
- Custom mouse follower cursor
- Magnetic button effects
- Video container cursor with play/pause toggle

🖼️ **Image Effects**
- Gooey distortion effects on portfolio images
- Dynamic webpack-powered image manipulation
- Smooth transitions and hover states

📱 **Responsive Navigation**
- Clean header with logo and nav links
- Footer with contact information and social links

---

## 🛠️ Tech Stack

### Core Technologies
- **HTML5** - Semantic markup
- **CSS3** - Modern styling with animations
- **JavaScript (Vanilla)** - No frameworks, pure ES6+

### External Libraries & CDNs

| Library | Purpose | Version |
|---------|---------|---------|
| [Locomotive Scroll](https://locomotivemtl.github.io/locomotive-scroll/) | Smooth scrolling engine | 3.5.4 |
| [GSAP](https://greensock.com/gsap/) | Animation library | 3.12.2 |
| [GSAP ScrollTrigger](https://greensock.com/scrolltrigger/) | Scroll-based animations | 3.12.2 |
| [Shery.js](https://github.com/aayushchouhan24/sheryjs) | WebGL image effects | Latest |
| [Three.js](https://threejs.org/) | 3D graphics (ES Module) | 0.155.0 |
| [Remix Icon](https://remixicon.com/) | Icon library | 3.5.0 |

---

## 📁 Project Structure

```
obys-clone/
├── index.html          # Main HTML file
├── style.css          # Global styles & animations
├── script.js          # JavaScript animations & interactions
├── README.md          # This file
├── assets/
│   ├── favicon.png.png
│   ├── img1-1.jpg through img4-2.jpg  # Portfolio images
│   └── favicon_io.zip
└── fonts/
    ├── plain-regular-webfont.ttf
    ├── silkserif-regularitalic-webfont.ttf
    └── KFO7CnqEu92Fr1ME7kSn66aGLdTylUAMa3yUBHMdazQ.ttf
```

---

## 🎯 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Simple HTTP server (for local development)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Aman2004-ai/Obys-Agency-clone.git
   cd obys-clone
   ```

2. **Run a local server**

   Using Python 3:
   ```bash
   python -m http.server 5500
   ```

   Using Python 2:
   ```bash
   python -m SimpleHTTPServer 5500
   ```

   Using Node.js (with `http-server`):
   ```bash
   npx http-server -p 5500
   ```

   Using VS Code Live Server extension:
   - Right-click on `index.html` → "Open with Live Server"

3. **Open in browser**
   ```
   http://localhost:5500
   ```

---

## 📋 Features in Detail

### 1. **Loader Animation** (First Page)
- Animated counter showing "00 - 100"
- Staggered text animations
- Font family transitions

### 2. **Page 1 - Hero Section**
- Navigation with logo and links
- Large animated hero text
- Parallax scrolling effect
- Interactive flag cursor on hover

### 3. **Page 2 - Video Section**
- Embedded video with custom play/pause cursor
- Smooth cursor tracking
- Video overlay effects

### 4. **Page 3 - Projects Portfolio**
- Grid layout with gooey image distortions
- Interactive circle elements with hover animations
- ScrollTrigger-based animations

### 5. **Page 4 - About Section**
- Text content with smooth scroll effects
- Image and text layout
- Contact email link

### 6. **Page 5 - Footer**
- Social media links
- Address information
- Copyright notice
- Character-by-character text animations

---

## 🎮 Interactive Elements

### Mouse Follower
- Custom cursor that follows mouse movement
- Magnetic effects on navigation items
- Scale and opacity transitions

### Video Controls
- Click to play/pause
- Cursor changes to show state
- Custom play/pause indicators

### Portfolio Images
- Gooey distortion on hover (Shery.js effect)
- Smooth image transitions
- ScrollTrigger animations

---

## 🔧 Key Functions in `script.js`

```javascript
locomotiveAnimation()   // Initialize smooth scrolling
loadingAnimation()      // Loader animations
cursorAnimation()       // Mouse follower & interactions
sheryAnimation()        // Image distortion effects
flagAnimation()         // Flag cursor effects
footerAnimation()       // Footer text animations
```

---

## 📝 Customization

### Change Colors
Edit `style.css` color values:
```css
:root {
    background-color: #030303;  /* Dark background */
    color: #fff;                 /* White text */
}
```

### Modify Animation Timing
Adjust GSAP animations in `script.js`:
```javascript
duration: 0.6,      // Animation duration in seconds
delay: 0.5,         // Delay before animation starts
stagger: 0.25,      // Stagger between elements
```

### Update Content
Edit text directly in `index.html` or modify image paths in `assets/` folder.

---

## 🚨 Known Issues & Fixes

### Font Files Not Loading
**Issue:** 404 errors for `plain-light-webfont.ttf` and `silkserif-lightitalic-webfont.ttf`

**Solution:** Only these fonts are available:
- `plain-regular-webfont.ttf`
- `silkserif-regularitalic-webfont.ttf`

CSS has been updated to use the available fonts.

### Three.js Deprecation Warning
**Issue:** Console warning about deprecated Three.js build

**Solution:** Using ES Module import instead of global build (r150+ compliant)

### Shery.js Not Initializing
**Issue:** `Shery is not defined` error

**Solution:** Scripts load with `defer` attribute to ensure proper initialization order

---

## 📱 Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome/Edge | ✅ Full Support |
| Firefox | ✅ Full Support |
| Safari | ✅ Full Support |
| IE 11 | ❌ Not Supported |

---

## 🎓 Learning Resources

This project demonstrates:
- **Babel & ES6+** - Modern JavaScript features
- **CSS Grid & Flexbox** - Responsive layouts
- **Animation Principles** - Staggering, easing, timing
- **Performance Optimization** - Smooth 60fps animations
- **Module Loading** - ES Module imports

---

## 📄 License

This is a clone project created for educational purposes. Original design by [Obys Agency](https://obys.agency/).

---

## 🤝 Contributing

Feel free to fork this project and submit pull requests for improvements!

### Suggestions for Enhancement
- [ ] Convert to TypeScript
- [ ] Add SEO meta tags
- [ ] Implement lazy loading for images
- [ ] Add accessibility improvements (ARIA labels)
- [ ] Mobile touch event optimizations

---

## 👤 Author

**Aman** - [GitHub Profile](https://github.com/Aman2004-ai)

---

## 📞 Contact & Support

- **Email:** info@obys.agency (Original agency)
- **Repository:** [Obys-Agency-clone](https://github.com/Aman2004-ai/Obys-Agency-clone)

---

## 🙏 Credits

- Original design inspiration: [Obys Agency](https://obys.agency/)
- Animation libraries: GSAP, Locomotive Scroll, Shery.js
- Icons: Remix Icon

---

**Last Updated:** February 17, 2026  
**Status:** Active & Maintained
