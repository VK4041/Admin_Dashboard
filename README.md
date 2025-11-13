# Admin Dashboard

**Live Preview:** [https://vk4041.github.io/Admin_Dashboard/](https://vk4041.github.io/Admin_Dashboard/)

A responsive admin dashboard layout built with CSS Grid and Flexbox, featuring a sidebar navigation, header with search, project cards, announcements, and trending section.

## 🎨 Preview

<img width="1875" height="911" alt="image" src="https://github.com/user-attachments/assets/78a27329-98f4-4e2a-aa56-5c95a05a7d3e" />

## ✨ Features

- **CSS Grid Layout**: Main layout structure with sidebar, header, content, and footer
- **Flexbox Components**: Internal component alignment and spacing
- **Responsive Design**: Clean and modern interface
- **Interactive Elements**: Hover effects on buttons and inputs
- **SVG Icons**: Material Design icons throughout
- **Project Cards**: Grid-based card layout with action buttons
- **Info Sections**: Announcements and trending displays

## 🏗️ Layout Structure

```
┌─────────────┬────────────────────────┐
│             │       Header           │
│   Sidebar   ├────────────────────────┤
│             │                        │
│             │       Content          │
│             │  (Projects + Info)     │
├─────────────┴────────────────────────┤
│              Footer                  │
└──────────────────────────────────────┘
```

### Grid Configuration
- **Columns**: `1fr 4fr` (Sidebar : Content)
- **Rows**: `3fr 10fr 1fr` (Header : Content : Footer)

## 🎯 Components

### Sidebar
- Dashboard title with icon
- Navigation menu with 9 items (Home, Profile, Messages, History, Tasks, Communities, Settings, Support, Privacy)
- Grouped navigation sections

### Header
- **Top Bar**: Search input + Profile section with notification bell
- **Bottom Bar**: User greeting + Action buttons (New, Upload, Share)

### Content Area
- **Projects Grid**: 6 project cards with:
  - Title and description
  - Action buttons (Star, View, Fork)
  - Orange left border accent
- **Info Display**:
  - Announcements (3 items)
  - Trending (4 user profiles)

### Footer
- Copyright notice
- GitHub link

## 🎨 Color Scheme

```css
--blue: rgb(39, 158, 255)      /* Primary - Sidebar */
--white: #ffffff                /* Background */
--grey: rgb(214, 209, 209)      /* Content area */
--orange: rgb(219, 153, 11)     /* Accents */
```

## 🚀 Getting Started

### Clone the repository
```bash
git clone https://github.com/VK4041/Admin_Dashboard.git
cd Admin_Dashboard
```

### Open in browser
Simply open `index.html` in your web browser, or use a local server:
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve
```

## 📁 Project Structure

```
Admin_Dashboard/
├── index.html          # Main HTML structure
├── styles.css          # CSS Grid + Flexbox styling
└── images/             # Profile images and icons
    ├── my-profile-logo.jpg
    ├── profile-logo-1.svg
    ├── profile-logo-2.svg
    ├── profile-logo-3.jpg
    └── github-logo.png
```

## 💡 Key Techniques

### CSS Grid
```css
.container {
    display: grid;
    grid-template-areas:
        "sidebar header"
        "sidebar contents"
        "sidebar footer";
    grid-template-columns: 1fr 4fr;
    grid-template-rows: 3fr 10fr 1fr;
}
```

### Flexbox Components
- Sidebar navigation alignment
- Header search bar and profile
- Project card internal layout
- Trending items row layout

### Responsive Cards
```css
.projects .card-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 1rem;
}
```

## 🎓 Learning Goals

This project demonstrates:
- ✅ CSS Grid for complex layouts
- ✅ Flexbox for component alignment
- ✅ Combining Grid and Flexbox effectively
- ✅ Responsive card layouts with `auto-fit`
- ✅ CSS custom properties (variables)
- ✅ SVG icon integration
- ✅ Hover and active states


## 📱 Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Opera (latest)

## 📄 License

This project is open source and available under the MIT License.

## 👨‍💻 Author

**Varun Kumar** - [@VK4041](https://github.com/VK4041)

---

**Note**: This is a static layout demonstration. No backend functionality or data persistence is implemented yet.
