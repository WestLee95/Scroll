# Nairobi - Horizontal Scrolling Website

A stunning, interactive website showcasing Nairobi with smooth horizontal scrolling animations and immersive visual experiences.
<span style="text-shadow: 0 0 5px #00ff00, 0 0 10px #00ff00;">
Not yet fully responsive, best on Desktop.
</span> 

## 🌟 Features

- **Horizontal Scrolling Navigation**: Smooth wheel-based horizontal scrolling between sections
- **Masked Text Effect**: First section features "NAIROBI" text with image masking
- **Interactive Progress Bar**: Real-time progress indicator that follows scroll position
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Touch Support**: Swipe gestures for mobile navigation
- **Keyboard Navigation**: Arrow key support for accessibility
- **GSAP Animations**: Professional-grade animations and transitions
- **Custom Typography**: Beautiful Google Fonts integration

## 🎨 Design Highlights

- **Typography**: 
  - Monoton font for the main "NAIROBI" title
  - Imprima font for section headings
  - Bad Script font for descriptive text
- **Visual Effects**: 
  - Text masking with background images
  - Backdrop blur effects
  - Smooth cursor following (desktop)
  - Pulsing scroll indicators

## 📁 Project Structure

```
nairobi-website/
├── index.html          # Main HTML file
├── assets/             # Image assets folder
│   ├── nai1.jpg        # Masked text background
│   ├── nai2.jpg        # Business hub section
│   ├── nai3.jpg        # Wildlife section
│   └── nai4.jpg        # Cultural section
└── README.md           # This file
```

## 🚀 Getting Started

### Prerequisites

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Local web server (recommended for best performance)

### Installation

1. **Clone or download** the project files
2. **Add your images** to the `assets/` folder:
   - `nai1.jpg` - Nairobi cityscape for text masking
   - `nai2.jpg` - Business/technology themed image
   - `nai3.jpg` - Wildlife/nature themed image
   - `nai4.jpg` - Cultural/heritage themed image
3. **Serve the files** using a local web server

### Running Locally

**Option 1: Python Server**
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

**Option 2: Node.js Server**
```bash
npx serve .
```

**Option 3: VS Code Live Server**
- Install Live Server extension
- Right-click `index.html` → "Open with Live Server"

## 🎯 Navigation Controls

### Desktop
- **Mouse Wheel**: Scroll up/down to navigate left/right
- **Arrow Keys**: ← → for section navigation
- **Mouse Movement**: Custom cursor following effect

### Mobile/Touch
- **Swipe Gestures**: Swipe left/right to navigate
- **Touch Optimized**: Responsive touch interactions

## ⚙️ Customization

### Scroll Speed
Adjust the scroll animation duration in the `scrollToSection` function:
```javascript
duration: 1.2, // Lower = faster, Higher = slower
```

### Content Sections
Each section can be customized in the HTML:
```html
<div class="section section-2 content-section flex justify-left items-center">
    <div class="content-overlay">
        <h2 class="section-title">YOUR TITLE</h2>
        <p class="section-text">Your content here...</p>
    </div>
</div>
```

### Background Images
Update the CSS background images:
```css
.section-2 { background-image: url('assets/your-image.jpg'); }
```

### Typography
Modify font families in the CSS:
```css
.mask-text { font-family: "Monoton", sans-serif; }
.section-title { font-family: "Imprima", sans-serif; }
.section-text { font-family: 'Bad Script', cursive; }
```

## 🛠️ Technical Details

### Dependencies
- **GSAP 3.12.2**: Animation library
- **ScrollTrigger**: GSAP plugin for scroll-based animations
- **Tailwind CSS**: Utility-first CSS framework
- **Google Fonts**: Custom typography

### Browser Support
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

### Performance Features
- CSS `will-change` optimizations
- GPU-accelerated transforms
- Efficient event handling
- Smooth 60fps animations

## 📱 Responsive Breakpoints

- **Desktop**: > 768px (Full experience with cursor effects)
- **Tablet**: 481px - 768px (Touch navigation)
- **Mobile**: < 480px (Optimized touch interface)

## 🎨 Sections Overview

1. **Hero Section**: Masked "NAIROBI" text with cityscape background
2. **Wildlife Capital**: Showcases Nairobi National Park
3. **Business Hub**: Highlights the "Silicon Savannah" tech scene
4. **Cultural Melting Pot**: Celebrates diverse heritage and culture

## 🔧 Troubleshooting

### Images Not Loading
- Ensure images are in the `assets/` folder
- Check file names match CSS references
- Verify image formats (JPG, PNG, WebP supported)

### Animations Not Working
- Check browser console for JavaScript errors
- Ensure GSAP CDN links are accessible
- Verify internet connection for CDN resources

### Touch Navigation Issues
- Test on actual mobile devices
- Check for JavaScript errors in mobile browser console
- Ensure touch events aren't being blocked

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 📞 Support

For questions or support, please open an issue in the project repository.

---

**Made with ❤️ showcasing the beauty of Nairobi, Kenya**
