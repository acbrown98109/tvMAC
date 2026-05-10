# StreamHub — Safari 4K Entertainment Center

**by ApPotato**  
*A sole proprietorship of Aaron C. Brown*

---

A unified streaming hub optimized for **Safari on macOS** with **FairPlay DRM support** for 4K playback.

## ✨ Features

- **🎬 3D Carousel Interface** — Smooth card-based navigation
- **🔍 Universal Search** — Search across all streaming services
- **🎤 Voice Control** — "Open Netflix", "Search for Stranger Things"
- **🖱️ TV-Style UI** — Custom cursor, keyboard navigation
- **📱 Desktop Shortcut** — Add to Desktop/Dock like a native app
- **⚡ Safari-Optimized** — Full 4K via FairPlay L1 DRM
- **✅ FIXED: Smooth Icons** — Removed grid artifact overlay

---

## 🚀 Installation

### Step 1: Host the Files

**Option A: Local Server (for testing)**
```bash
cd streaming-hub-safari
python3 -m http.server 8080
# Open http://localhost:8080 in Safari
```

**Option B: Web Host (for permanent use)**
Upload all files to any web server or GitHub Pages.

### Step 2: Add to Desktop (macOS)

1. Open `index.html` in **Safari**
2. Click **Share** button → **Add to Dock**
3. Name it "StreamHub"
4. Icon appears on Desktop and Dock

**Now you have a TV-style launcher on your desktop!**

---

## 🎮 Controls

### Keyboard
- **Arrow Left/Right** — Navigate services
- **Enter** — Launch selected service
- **Spacebar** — Voice control
- **M** — Menu
- **Escape** — Back/Close

### Voice Commands
- "Open Netflix"
- "Search for The Last of Us"
- "Next" / "Previous"
- "Menu"

### Mouse
- **Click service** — Launch
- **Click dots** — Jump to service

---

## 🔧 What Was Fixed

### Original Issue: Faint Grid on Icons

**Problem:** Line 29 in original code had:
```css
.cbg::before {
  background-image: repeating-linear-gradient(
    0deg,
    transparent,
    transparent 44px,
    rgba(255,255,255,.018) 44px,
    rgba(255,255,255,.018) 46px
  );
}
```

This created **scanline artifacts** visible on service logos.

**Solution:** Replaced with smooth gradient:
```css
.cbg::before {
  background: linear-gradient(
    0deg,
    rgba(0,0,0,.9) 0%,
    rgba(0,0,0,.1) 60%,
    transparent
  );
}
```

**Result:** Icons are now perfectly smooth with no grid pattern.

### Additional Improvements

1. **Safari-specific image rendering**
   ```css
   .clogo {
     image-rendering: -webkit-optimize-contrast;
     -webkit-font-smoothing: antialiased;
   }
   ```

2. **PWA manifest** for Add to Desktop

3. **FairPlay DRM optimization** — Opens services in same window

---

## 🎯 Why Safari?

| Feature | Safari (macOS) | Chrome (macOS) |
|---------|----------------|----------------|
| **DRM Level** | FairPlay L1 | Widevine L3 |
| **Max Resolution** | **4K HDR** | 720p |
| **Netflix** | 4K ✅ | 720p |
| **Disney+** | 4K ✅ | 720p |
| **Prime Video** | 4K ✅ | 720p |

Safari uses **hardware DRM via Secure Enclave** → full 4K support.

---

## 📂 File Structure

```
streaming-hub-safari/
├── index.html          # Main app (3D carousel UI)
├── manifest.json       # PWA config for desktop shortcut
├── icon-512.svg        # App icon (smooth, no artifacts)
└── README.md           # This file
```

---

## 🎨 Customization

### Add More Services

Edit the `SVCS` array in `index.html`:

```javascript
const SVCS = [
  {id:'yourservice', name:'Your Service', url:'https://example.com', 
   logo:'https://cdn.example.com/logo.svg', color:'#ff0000'},
  // ... existing services
];
```

### Change Theme Color

Update CSS variable:
```css
:root {
  --glow: #00d4ff; /* Change to any hex color */
}
```

---

## 🐛 Troubleshooting

**Desktop shortcut not appearing?**
- Make sure you're using **Safari** (not Chrome)
- Try Share → **Add to Home Screen** instead of Add to Dock

**Voice control not working?**
- Safari → Settings → Websites → Microphone → Allow for this site
- Press **Spacebar** to activate

**Icons still look blurry?**
- Hard refresh: **Cmd + Shift + R**
- Clear Safari cache

---

## 📝 Credits

- **Created by:** Aaron C. Brown / ApPotato
- Original Kodi addon concept: StreamHub 4.3.0
- Converted to pure Safari web app
- Fixed grid artifact issue
- Added PWA desktop shortcut support

**ApPotato:** Code · Design · Innovation

---

**Enjoy 4K streaming with a unified TV-style interface!** 🎬
