# Theme Options

This site features 5 unique visual themes plus a default light theme, all accessible from the navigation bar. Each theme is inspired by different design aesthetics that complement an aerospace engineer's style.

## Available Themes

### 1. **Default** (Light Mode)
- Clean, minimal design
- High readability
- Professional appearance
- Perfect for extended reading

**Aesthetic**: Classic, minimal, professional

---

### 2. **Neobrutalism** (Brutal)
- Bold, thick borders (4px)
- Stark contrasts with black outlines
- Bright accent colors (yellow, cyan, magenta, neon green)
- Strong shadows (6-8px offset)
- Raw, unapologetic design
- Grid background pattern

**Aesthetic**: Bold, raw, brutalist architecture-inspired

**Best for**: Making a strong visual statement

---

### 3. **Neomorphism** (Neomorph)
- Soft, subtle shadows
- Elegant depth effects
- Smooth, rounded corners (20px radius)
- Muted color palette
- Inset/outset shadow effects
- Gradient accents

**Aesthetic**: Soft, modern, elegant

**Best for**: Sophisticated, clean look with depth

---

### 4. **Techno/Cyberpunk** (Techno)
- Neon colors (cyan, magenta, green)
- Grid background pattern
- Glowing effects and shadows
- Dark background (#0a0e27)
- Digital/futuristic feel
- Pulsing animations
- Transparent overlays with backdrop blur

**Aesthetic**: Futuristic, digital, cyberpunk-inspired

**Best for**: Tech-focused, cutting-edge presentation

---

### 5. **Mission Control** (Mission)
- Professional aerospace aesthetic
- Monospace typography (Courier New)
- Data-focused design
- Terminal-inspired elements
- Color-coded system states
- Bracket decorations `[ ]`
- Status indicators
- Military/aerospace command center vibes

**Aesthetic**: Technical, professional, aerospace command center

**Best for**: Showcasing technical/engineering projects

**Key Features**:
- Prefix decorators `▸` and `[ ]` for emphasis
- "// " comment-style section headers
- Terminal-style color coding (blue: links, green: success, orange: warning)
- Uppercase text styling for buttons

---

### 6. **Retro Space Program** (Retro)
- Vintage NASA/Soviet space program aesthetic
- Classic space agency colors (NASA blue #0b3d91, NASA red #fc3d21)
- Aged paper background
- Bold, uppercase typography
- Box shadows and borders
- Courier New monospace font
- Classified stamp watermark
- Vintage technical manual feel

**Aesthetic**: Vintage, historical, space program heritage

**Best for**: Nostalgic, heritage-focused presentation

**Key Features**:
- NASA red and blue color scheme
- Decorative elements `◆`
- Uppercase section headings
- Technical manual styling
- Vintage stamp effects

---

## How to Switch Themes

### Desktop
Click any theme name in the navigation bar at the top of the page:
- **Default** | **Brutal** | **Neomorph** | **Techno** | **Mission** | **Retro**

The active theme will be highlighted.

### Mobile
1. Tap the hamburger menu (☰) in the top-left corner
2. Select your preferred theme from the list
3. The menu will close automatically and the theme will apply

### Persistence
Your theme choice is saved in your browser's local storage, so it will persist across sessions and page reloads.

---

## Design Philosophy

Each theme is designed to:
1. Maintain full functionality across all elements
2. Provide excellent readability
3. Showcase different design aesthetics
4. Complement aerospace/engineering content
5. Work seamlessly on all devices

The themes were specifically chosen to reflect:
- **Modern design trends** (Neobrutalism, Neomorphism)
- **Tech/engineering culture** (Techno, Mission Control)
- **Aerospace heritage** (Retro Space Program)

---

## Technical Implementation

Themes are implemented using:
- CSS custom properties (variables)
- Data attributes (`data-theme="..."`)
- Modular CSS files per theme
- JavaScript for dynamic switching
- localStorage for persistence

All themes are loaded simultaneously but only the active theme's styles apply based on the `data-theme` attribute on the `<body>` element.

---

## Customization

To add your own theme:

1. Create a new CSS file: `css/theme-yourtheme.css`
2. Define styles using the `[data-theme="yourtheme"]` selector
3. Link the CSS file in `_layouts/default.html`
4. Add a navigation link with `onclick="switchTheme('yourtheme')"`

Example:
```css
[data-theme="yourtheme"] {
    --bg-color: #yourcolor;
    --text-accent: #youraccentcolor;
    /* ... more variables */
}
```

